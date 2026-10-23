代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jqlekfsz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rqweozjs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lvzncbyy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wdtddvyn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzvwsnjb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uyssjasf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rybfjxkf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nkuwmblr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fhitujnv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pvjvifum.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bwtvpwkk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xkvswtsj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yoaxvieb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxwbbluu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3yilfngwv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfopkvfo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3raltrtse.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3eqnijkxv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cmuezdju.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aiixclhw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxrwyd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3alpgspuk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3snwqdmev.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jelsmxyi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3eglfmgbm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vuzhcxez.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bfpzvakv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3guowszuo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cfwswnok.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yqekbjsz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fphczhba.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3irrqgmzu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dcgmafel.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nxqfychk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3iqzwqfyj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3cobzoxrj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xzltpchy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csissfbi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iufkpluv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bxrnipbx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hbgcciax.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cddjdrsn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kuntotyv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nbxtgecm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tnkmyvvl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vflhcaft.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxpngwuu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xghsgefv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fnnuoaxu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwbrxpp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qohgthxc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nkijggli.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uwnebdfv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xpnzblsv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3aaopjdvb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqpgmzs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnedrunu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbzidec.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hnycnnlc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vpihuctb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvzclchd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3htmgzowv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wnypvtrm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xzotwxsq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsgjxtcb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tjhgcgun.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zkdkwcqn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wxibessf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gcgwizyw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ltsjyhhr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zirvqlbp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3myytnbrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zrcwtwda.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqplqenl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ddnzalap.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qlimrgvp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3cvdmblyk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzwrgfcc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfppgltq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xvfgkrpq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ylpifozh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3usmykwmr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ureuhtjw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tybvfbdz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dcypzpnh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3maksqdzd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mlzxybsr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqbnzim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etcogmsm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iljyhwfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cstlvmew.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ekpjwlae.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hivgnwpd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xlfftywe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzaqidj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bkxmdhky.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pjbvadgg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3owmghvzj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3eserguuv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qmjqnhht.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yyvrgxbp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xnsblaeu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vsvsxxgs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qfbkewms.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kscxorrx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ibhntszd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmmkgesx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3edssavfb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3eoiiboqz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qoqcakuy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lkwxepvt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zojniedy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3euvfobhk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zsvoqtod.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lwqyckjd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bnucdljx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rsfmzrmr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvfxbpl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uxokwwjg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbpvscn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pniewiwi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3olrxoffe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jdxtcdjq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uvrcmhyx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hkszbqku.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qxtdbdde.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlzpczoj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jmgkvipw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xdwisune.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3krdrtzwx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3clldcfbx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tzmqxasm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gqyolluh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ekgzhfld.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3efkcagwr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eytvelqg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yjxgwfva.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kxtoxgiz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pogwfifi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lcuvexoj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3avkzapeu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qstrqxrc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hgmpgybn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ekqpojgv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bbitlwrw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qwpjaomw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fxnilsgb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipacqnuc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xdbugcjo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pybnvbqm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jcwoqiza.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dvpxbdjq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ybrpcpbk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ozjavsxd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3slplzced.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfmopcl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pinvxtak.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jjibguek.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gljxzajt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vblkcpta.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mnfscusd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qsnfamiy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bpvrmqru.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zptxcamq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqjksgpy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bhycasho.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3abcmvmgp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xgqaknny.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eplsmorb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3boyqyvyn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cvvjoxhb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ybvlczjl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rvtjchhe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nkqjsvwh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qmsvcjnt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qiowfksh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3afjaqmir.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3aikwfqyq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ehscufyd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yvaavsaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ngpqcvfu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptlwngii.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eykjxfod.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gmryuuse.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dhiagwxn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3minmktex.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mfaqpzsc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ueferxhf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rfnbsrsd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oiyvneul.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vixabukm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3okcsnepm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3pntsjanx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdoqfawd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hewdavxa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pqnpwttp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3chaccaqg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rctbxzrl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3flfxulzi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ofyhvxfi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hesuzley.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3egnckiha.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfuypcyf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmvrksdd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3homqrsgr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fggvrjma.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gjdtzrmq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gmysmefv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rvdekudg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ljhizxuv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jxcdddcf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dyfxfgcv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3igrjurgm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rttrjxxc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dwsvmwea.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ujdazrbu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fvctvuvx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xgzzofet.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwuffdgv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3abxbmnvz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgebnjv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zzmkxazi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3sefqxkrd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfwzspw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlpgfcuh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3erxavnny.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3imaqjkxh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uxdtrdea.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ebplytdl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hzztzbtt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pfiupnnt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3leidhxsx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yukxfzft.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gznuzgzr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gnhehpkx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3guzikwba.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mybvyjno.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ddnyxvde.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3psawhgro.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3skbgyqdi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bjgvwtcr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uvhkyemh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bbabmgri.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uvagrndx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3srmjkirl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ndimvnae.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3msevclyk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iegyowmb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mcwvwiez.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxlqzefi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hbrvltwh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ltlrgubj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ucyyycev.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fdxbzsgv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gksbffgs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3whqiejma.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ixqgthpr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bdmkpcuu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kchuilcb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3escqvdql.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ihtmlclf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hcjegrxk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fccfbvni.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nqvlkuik.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3llwlqyjk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csxnbfmg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3skdhdnas.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3aaazeumt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hlmaypfq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kxmizrtm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aphdoesk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fjccpphb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3spseqqzn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hqzdhpfc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uqdecxzv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sfvuhtri.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aficzybl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xosdevhm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ihyisadm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rghwnucw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fvhfikcc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olyflqcs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rcxhzzdp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rlfvjaan.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3exbizydr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gxvutdqj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3aponslnh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3buxypbdi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mxoxxmdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3segygndu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3efdmnpju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dptnnfyk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxuwlslc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3bjkuacll.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ddqbjszp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jcioqkuf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ktlvaujk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fbssqdvh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3uotwmofq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubztkkkc.html


<!-- 参考信息 -->