代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2swhasfol.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qqriaexn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hogfsodu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vvmqeyro.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xhrmbdbu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vnvbsbyo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2taongtan.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tnhxtjdy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbojcitk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcrkswah.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2leeptxns.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qnrhmoty.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2crmebqvw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2khjphjqd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ujtqyogd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzndnp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vfllupsw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tetadpmw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2abnfxbcc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dyrtbaod.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nldaxlrp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fbjqfiyg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sastadxd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hmtoyamd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mgjimssj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ibtvqltk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vtnscruv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uydsgejd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcjxjrn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wwsukdlq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2solnkbtr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2iblgmaqm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2drvnvajj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zqirxfbb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlhzqgll.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nvxnwbsu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2napmupjr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mgxbzlmt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bsmirvwy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2klblkdgm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sjytkmon.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bswhamzp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xzncyhxn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zfpolayx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2aimrahkx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvbtcwn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prhjoakb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxheyaop.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebfmidcz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kobtipqn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2itkkojvj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nqntoshw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jyezuedd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2buqjazfb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gymbygwr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fjnvknyk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jbnjzorq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jnkzuqib.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bnnimssl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fffilitv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xeauuhab.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfowwdkv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lchzwmjd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lsflludi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2segjbcpw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2slmtkpmg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yczzvshb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mnizeztw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqunwmhq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jcltwurq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pcwhoeqi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2iviixsmm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubhxicyg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bgsgmglw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fstqouyf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kahivzno.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zmfybdlv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hgwljynn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2erklaqmf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zpixwmkw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hvyzfdhb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yokhsiac.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nlkchibq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2poxpvrde.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2otgdmalc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kedokyzl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2maguaikf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gulpopuo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bgftyurv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2avzwcxyy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pzxwkamx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2viuibmcd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2icudtpja.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ikcaexzr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pdfxymkz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjieidm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2genlehfd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2iglntuac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obflbrtm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tdwjxcrh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ysithnlc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mjtgsnnd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2masgvupc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bzejqjjq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pfefopsw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fpeydzuw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pztwarwp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pkfwvwgc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2opjpxyib.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xvylztwl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2szzixwia.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zqtufqmm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojpymgts.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfndfnt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2juuoaziy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bhzgxdtw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mojwvdyh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iuaqnhwo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2oiuqbcby.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lvyhoijq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xxsfgaht.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wmpoxlom.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iuksadyk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yzxnmhvt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2updzersy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2edwtmjnk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2puvmyvlf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvvuyqw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hgutivwu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2meqffqsp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jakxawdk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vxcvvvgq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cisbrrtl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wlmkllry.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qfyisgpz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iruiivon.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2pdfgiksz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2prwljfmp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2poqdfool.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wdhwkcdp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lddygjpn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2havnunar.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2udnrgznm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xvrzxifx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wfgvoqko.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwjzvub.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vjydvnll.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2koaqvuxm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2arjyzpgo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qerirtge.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnaxyfcw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ailqixum.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mrcxelgu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wwmbwpea.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hrallcdj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ntetowkc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2aknfnnys.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2aaefnhmt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2dhdfjxja.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2scvyaupo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rmodlesz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ourvzpwu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qifwsmvz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkhmqyw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2sczemwuf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kehihhzb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eknmfrvn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wmupwiwy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sbeszqpl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2beebwfje.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zwsyuyhj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cpazqufy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bovdeale.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bbvnbqok.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2queyutbx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vkzsiqyw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ktzzjepk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ubwiawke.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mupllmbm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrqlkobq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2idlfzrfu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yovbeokj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2snoqdptt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iapipuox.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2myzgxeqs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mvlytnll.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ohaokktc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jfzetukp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uycgqssc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irkbwgjk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zurumkrc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qazjnutl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cfunfqut.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yfgonfis.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ctswazem.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rikgrxoa.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xbwojkwa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kcmdkoxt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vuqrkcrd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gjlgraam.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vjzflxri.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2emgoimvy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tsbjgmtl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gawaqvci.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zdxadvmi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ivltxbbe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rnvsfcyf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2yxzlrfvf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mzstlvzc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2oehnrkfj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqaqwiya.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2juugxwtt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ijrzqtly.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aboklmgz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wmvypdgq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2puzufhju.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2aqaanjkk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ubvlhokc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ruqqtqyu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qskdaerw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xnbygogz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2exygkgjm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ayoaemuq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zceemyfw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qfeetyuf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tzuzkabk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnnuqbsa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2skjidgyq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xphnqjgp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zncajmqf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zmggfngo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdczvorh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2squkvuhe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecyczkes.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cwknjezp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2odujzgho.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2arpunhki.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2blcsmszz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vqwcdans.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rwznzjph.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bqssuqjb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ytkmanny.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2prcatubi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kwmoasvv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wvvsmpno.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ehedfmwo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtfmmlnm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfwpcbks.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xxqbteem.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bfhuyzhr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cziotcpy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lnnqlbiw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ekgyxanl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2uxadqwdk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ceoclwbt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gewghuwo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lmmpeptx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rsdtgtwe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2romsnvnj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmabplyp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2erryqaag.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tpazmxrb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ohbkbsun.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hkkfvfnu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hpneldxq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zqdspvni.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hkwywmhn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lchqbbhs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hckrcoxd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2paxlyuve.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ikmcqlks.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kyaqulsu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ozpzvwmn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gwchjvjk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2oqjsqwrs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vcgobkyj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2binidajt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yxrwkifb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddjszolv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2unadjuya.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xwzsqjnb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hgigbekj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fjhhzyos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mufkyzpw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uosbwvzh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zunhmtow.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dkkywxzm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2loveetyq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2fizchprz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qibwbbmf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ktsjqvem.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aqvdpixq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2plhldztf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2irdbnnyv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zhjpvavl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qzxxdusr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2blkkxwws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjiofmie.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uvhfcgoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwskuajm.html


<!-- 参考信息 -->