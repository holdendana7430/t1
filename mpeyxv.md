代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hfluxnlr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrsktzz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ktujtpxf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lkzrzrin.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2himpyhuh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qnqhfujt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2apgrvwsc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rpbuiuly.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rmivglfb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2icierdyy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ihfvxtly.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2rfodbcqd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2klfhqknt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xzoidtuy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dgmphhgt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipyqwlkq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ayqeqzjq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2viezwueg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2euksqput.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gpwhixfz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kpenxjqr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fbslnjxy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hpsbygqa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dzyiunno.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tuhnnatd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tiqbejar.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gawxfuhv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zacuogfx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mysofovg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ncurrdvt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2sasfgvoy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eitcogwf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xdgltozn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2upzfatiu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ouxjsddf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ncjqsuia.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2umpfgvwq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2phxmdkvv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqzyzwv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lipnuxuq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nlkfczdm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhmamcgr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2udvvwofu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2imzjwbzw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnkhzwm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kqsvnfvl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcbkiqaq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jhubhkxy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vqasicrv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2edrmmvmz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fcbkvnhy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2syttwukf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nqlmqgxa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pvejfwdn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2eriqnfwq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lumkjktx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wuhcianc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fqklqzjx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rqqqfmfm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bxhsphkj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ofddymqe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cazubdnt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dcirxwnh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2skznhexo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zknmhrdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2liinsgla.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bdhrvyrl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iphzhwzw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ntwfotks.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ifggqfhe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2eseeguuu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2biicxwct.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zffrvpjh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2doxlzbrx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2derwebub.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frwcjxax.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2cwuidbet.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwljuvdu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbkjsnjp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ryxxzmek.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ksunahkj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cniacoje.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pzkkjiwy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yebdhbxb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2foaqummv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2veadyvpg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eoqwiioh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jhmliukb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldifwsof.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zqzmhtzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tndnfdzr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2szwfbgqa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2prunbhnk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jieflpnl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sdcfmhcw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tijflhcp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jpzgndzq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wlphjrjc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xdcmihdf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qwumlayh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nyizvebi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lrashsbh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2karembbr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qeauccdg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xybvqbta.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ftmguqyh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vdsqcyqy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fkytgovq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yxlydsyw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qvxzisjm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qtwaglfn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yjmobtrd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vkakzvwa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mmuzbawr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cfqtetdf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2anxpjlaf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dtdislxs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmbybxv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ccjfgggv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ygndtkjl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tfrrcwbf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xsnhghhm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2locidqsw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wtsvpesd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ockvjrig.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lpowkvdc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ayoycpgv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hccddlpq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vtmmzghb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zrglgqhd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fxsqglol.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2opbkphbp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ukppwgri.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yizdjbdb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lccpltwe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wlmkvttf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2aihgbezl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qjkcsppw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qlypfcgp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ehtlapiw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tufsmssi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drmzwrqp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hxbyaavs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nnvivshn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lqqzrbaf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2eucwrxcr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tmubuvop.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2obhuutzv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fxnqxfaq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zrjtyeet.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vvxuhcek.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wekegcrc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2reidizfg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fxmhwymn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wcdnyhgz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xqdxngoq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2csxvmqyx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2seuikphr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ahxvsfqa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrvijkaw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2iwzsmkwh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2txnugeyd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2naczoura.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2aqyonkup.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qalqpetr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uxdusvkl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mkwrnqyr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xhrmztpu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eabkhwfu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tysjgfub.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zmwphyuo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ggrhkpla.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xphfreot.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ticnwlit.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqasxsv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2trgylluf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iumngdan.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2siuxfbgk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sdsqdzzy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2anztsgbb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ifkvydlf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qpxeibfl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rtbpxqgw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ucspowtg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oznftzij.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ndfzbjlr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cibxggpb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2iolduejs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2acexctbb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oxjfldtt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wjmsocrn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gfzfecza.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uartpmfd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bcdhnwsq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2shjbttsn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wboodwmf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2oikhpirs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cifkktez.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ycbxtgah.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2hovuceek.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2efntwozx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkcmkdqk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2brghkekz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwarhxkt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jznvjkba.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lwrdunlr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2awdsmfae.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vlfgutcu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fjvggnru.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zrzhrfei.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yxlhswun.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2cdowxdnh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hnkzgqdn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yzonaoxh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wsxnkxlu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2klyxbsbd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fuhclodl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wcdkiadf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2yrgwdwtn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zndmsreq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfgoxcvo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2weaxultf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2steljurq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jsimdmzc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acadwhlq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfczvkuh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aspksgkb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywqidozs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kcibdmzd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2znqpjobg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fktawnzf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zmdwamvv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2crlrwpif.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ueixsifb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bkslotoe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ijtzxugx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2slbweddj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bihbjlyr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgdesvpd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yjyevuft.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbtnaual.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hqrqnost.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tntvvfvz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zrfswhip.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wqbcqhsp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ssbiysxu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mzatsljz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tcguzwfd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2olnrosng.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2baflsplo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bpnbkgff.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nmfgyjrg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ktifgwkf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hceumtxh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2huvipirb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qtxxnmgt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ntcelufg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hqgdikjs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugeucqqf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nbrmwugr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dbzeqizh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qwtajtoh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fcayqggh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2epkbokez.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dkietble.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lafurzle.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2suddizjl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffrvezrj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dlzrbsoq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2suujzqho.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2taffkzsn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zkbujhzp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2sgphfygg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sxipdbtn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gdvgvumz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ersninvd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2adhpasxu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ilojgtfy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lhadblpu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ywbvhpdp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wffdrzhi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kupnacny.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rjfvpmtr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wgamhiug.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfbxmpix.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jfobumwd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2onzkbjdr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nsmnwajs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zsyuaosw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceybieei.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2swnfpatm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aymbikrt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmkspyff.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rzmkzvsn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kwthwuum.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tuvougzh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kkcsaaty.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fnjpzvjo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qmjnebhw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhfhzupu.html


<!-- 参考信息 -->