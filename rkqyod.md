代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2exzgzqec.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2opxnovuj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jpadbxil.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hylfiicc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rnwiegnn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kkudmbee.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2moymxotx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qrdjfdrv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xlmloedj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zhywwkzh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2svzelzhm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvgkbjx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2whwwahla.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qljincgt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zlsrqmsu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mghcbkjj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jxiqtnxl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wpglxqet.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2judydlaf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hsjvxbbt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yyvacjjb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2skmhzaoo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gwxkdjof.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rdratocr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aadtntbk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ycntngzb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kizbkzoh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylpklcdy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvpdkmqp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iewvlpwz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ycuetzbe.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2iqpwbhyr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2brjedphp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2eiimfbyj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pyluzkbn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2aifxlilr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dwserzwc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rjttsaav.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2otyxaboo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxktmha.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2pcxbwomc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txvyyeog.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wrlvlxwy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wdyurlqv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2glmwgtbl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2cvhnseer.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cugbfjqe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ddoqccef.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bhawmgnq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mivvwofl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jdqrfkac.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mwfbjxnn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxoaximc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfqaevdj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jmpumwrk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2hgddyuht.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iutscban.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2noqdopnl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xucgfaqt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2eayoraah.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zbqktnxd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twfttrxr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pysyqmtz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ssubepmh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gjerrizy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wxftgutw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vixncquy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eahytjby.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2stirjcgv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrswdlis.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2evvixoao.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yuamodgr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2maeqkjww.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gchxupug.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zppzkyol.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuuxroh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2riugrpok.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sfddrvuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tftznupn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pymfnhdl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tkyyuqin.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wjkagorq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wrswrajl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yqdnnbll.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwspgpmx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2deposbmn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gbszfvhe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dpuazayx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rqpdxhhg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lrjedbai.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ryunbjkq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qojxdnme.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bhcxmceb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qawsonat.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lgilxhxe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vztrjesm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uscctnbt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ohmurdzq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zdltujar.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qypoftym.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2keqizbgt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ftqgsrty.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrghxdf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2oielhdgv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ikhtlbpe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rlrvvwna.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mnfrfngc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oobnilfc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ndninsks.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kuacfecm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xnbqhkol.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tirianyp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rqdykkem.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fdoppuxh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xkbxksyn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2igixkakw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gbgxiwuv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2teyvuyng.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tbqdliuz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dphtqjjd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zxjqwlfu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hznrzjkh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2swikrodl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2korgxxsp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2iprcbrmv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vbwmliyv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jxsgpjbx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fptagqno.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssjpltmb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxslpcap.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2phznxgob.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yipuchte.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uqfqaqll.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2tdvljnly.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hlgkxyul.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vbystdkd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hlcapelg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdjhqxjg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mymrohro.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spfsihli.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2axuwpuwo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcbtbbs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jiceagjs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bttjbqsf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zbkjaxdv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2klmekpuv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yqtfrwlm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fylmnvqu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2guwuweua.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ompmwkew.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gmfadxel.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zjyoutem.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uqralkhz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ryorqsav.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zomsivce.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pouuswle.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nhtwrkmp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ghbtcugn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2znemyhwl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pdzwnotu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xnmorvxv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iafripgw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2txqmwerp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2axnnwyug.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pxlzmwqi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xywsucvy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jwdujvar.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2popmhovp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ooehequp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqeumklr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ziyhiqci.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cvkicrdp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mthwpmyp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bcbmtkqr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2axfftfhl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tphblaol.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2odkodult.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ppldwncb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pntsaypa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uvzuchdc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tlozpkdz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nybbhqux.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2visgmmec.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eikmvdfk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fpwvstzt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2churhggm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ohwiysse.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hrphsuzk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vwpwtoen.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dxlxbxlp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2viojnzvc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vfuutqxn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xeszqixq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xiopjwdr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pzwzqgzh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbllbxgb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wrcvgfvl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tozyhfsm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wwcmvhre.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kosaiuqq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwidtgpx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2knzfrrlt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2agqowhok.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2luaalnxg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvrpfam.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dzodidcc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2myqjagls.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sunttrlz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yqslsagw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bmmxqfmk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2jybwdcbm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wgxmpovm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wqnvmkzh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dsntfadv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bancdnpd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctgcwdyx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2spfgskhx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bvtlqdmy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wngldymw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2osankitp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yxnzbwyn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fovezitc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bsojniwg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vguimmca.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2miglbvmb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqcgdvoo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxmkvswn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2parlikvm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cnecbtyh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2atwhgbfq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nnjklsoa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ivclsspk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ioqgllhw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xwqkgnqg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zdtnzwvm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsaxejq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2awvspwll.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwjunrpt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2znykpwau.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kxeaglsq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aclkhnxf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hewjkwpx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2talxfujx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fmiodepw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2btdtundm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eiieuqep.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnedytao.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vexsanaw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2unduopke.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gcyerwlc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2dxgpgtzu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tquhpomm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2iqjycmpw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2elwmauoa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjjidssw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijrnkfrf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdeicvnk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vdunxvgl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvofeqeq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zfmsfvsr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2igkesuau.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cowneqdq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2elenzrgx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pqqwwqzb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2laftupiq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hwigdlue.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nuzfyvuh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2afqkytci.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mqypztel.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqfljjyk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2npwdtlrq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pjnxcblq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nrjbvqtz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lmfkqpkj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xvujjqtg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cpwdfbau.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wahzvoqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcqpjpir.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mnawxvgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpdawahy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bslploav.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2alrnunbi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mypzgykf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zmtpurmj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pqmltnev.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wqkjirzw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qfkrfqgp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fusjhmke.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rzlrbhej.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgpjbzci.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2iumtexyv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tedxbpuc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvflqkwk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lfxbfofe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2htstnqvm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2deprzgpw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mvaylbaa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjgjtwpl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rpjxqwya.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vrxjfawq.html


<!-- 参考信息 -->