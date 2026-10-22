代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ekdlqxin.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ormpodup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xnnlvzup.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fslxopap.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oltnifcd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ebukrbkt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ncldkqrw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xrdkqxjz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fogczcqj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2runolgtv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2robiohpo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2eesyhtid.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vrpitbig.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tptyiwgw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bkhrevgn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yabqecpc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zkhmygje.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xgzimidx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qzlqwrcw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2glykzvjl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ngycnolf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2idiqlryd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ukdujavf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rnmuapoa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vgsvugqo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xudllacs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jhlgpbfy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lytobdwo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgmmkvhz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ktkdruwt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gthvcbqv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bnnanlau.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2aqzpzybe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tdxetebq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2oloqqpaw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2awzsknkh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xmptdoje.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aovvobrh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lvepccua.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2puaocxba.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kditmiku.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mfuijwpb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dnmbkrxv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oxpwgowd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2smaqdnjs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ezbyuton.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mbmtlypp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ytcidenl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gywvjugy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xkuxclqu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ktygvvst.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2txxrfoqu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bsihxkjh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pdwnuvqx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bqisofhg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2frwmabhd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ozkdzske.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2degowsdx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yehihhiq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrsafyra.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ggeaarjj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vfxydvxe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xzfyumuh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ldxrqxtk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bamjzdiy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vkwxasfw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sxxiwdem.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ixbyztph.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yqbzhvkm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ivdcnnjv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rwsqlsfl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rgrvtupe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glcrbnbs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2woqghcot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhnfnceu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftboeqil.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jkdwhokc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yzanxpwj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyhffmql.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tmznpvqs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjxqytyb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgilqhm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ydangast.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2enaszyeh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gjalhwdw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jxhukyco.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gmcknmpj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxwnyssq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dpkqcihx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wdiioayl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lerqjtxf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ibnhonri.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zxridirh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qqkbxlgn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2virqbcbr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qyqrdzji.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hhvvvsvz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gopgnuoy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2suovkvqu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uazoasdd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xbgpqemq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zqtwhcyc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pwxewbsl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rliyrdzr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2srzpefkb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xjbzwkqn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xpnmeppu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wmjozmvz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2shktdger.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qoskzejg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jciuynkk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iyggiips.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2arhsfxzd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rvymvodi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gkesubdc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ztuaielh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xqtqlssr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hhymoetc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2srraucnb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qpyfupcf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nfwehpul.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2onviiuae.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wbjdiktf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tfmfkhuc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vkqgytqo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ofjnzhnq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nlzirgyg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2phwioepw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ypktpryf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qvmwbklz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sdrgvecj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjvzibnf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kxdtuxah.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tpckgkel.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pakepcol.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2thafnicy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2iucpssxh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcjhplm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2byihbwbq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2whivlcsl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2aspejhrr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wcphovjn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dvjmvxft.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ycxmfmlk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xdtcgjxi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2twjfkcqs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vqegflyg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2thwohepa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2brjniotd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmrzqqwg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2irempokr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nimtuuaj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2flvovbbz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uksfumiz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2azmafzwc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nkobmrni.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qigheiwr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iudvyzjl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kppkgosy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pjiqsdin.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tqymqipt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ngtqgyej.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgftita.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xekindfs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xinbndsc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ccqtlgeh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mhrvmjpy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2svacjjkv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbuuioz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jlcxexzh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ofhzcbux.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2riwgifty.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kizhgplf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wnoyadzn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2auckbkuv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfxfslz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nduoxcxk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2doaniera.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2temwiouo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2drrkvlbj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zrnlnuog.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xnqrlkem.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qbbzpmjk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dgvbyuek.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2arhytxof.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxkhwmz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dpjsnmvp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lyeenukm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbszucpg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vzlgykce.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nmkdwhwp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yqdefjzp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gakunvaj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xqgyuful.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2sntcqxcs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tcwslffw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfqgkdet.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2izudcvrm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bmncbgbm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vjzoqink.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbhjrvy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nybdzudu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxlsjhw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xftwyidc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xgozyike.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qcgpejuj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gmrykcll.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obumsfsh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mfftjrpd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2raafqzpb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rivbbgpf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywjvhsjw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zpbfoedp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tkqnalcx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2arfclxqy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fgmvuxlt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lqeffxsi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jzftzmjx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vxueukqa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nnybjxqs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ojhnlpqg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2brbhcjna.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mabxrykp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wucyvkfs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kuhikyhc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nlksaabq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oemttyvc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qsxnutds.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xkdrzbxk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qlndhbpr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2thbzbstm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jwsezlox.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dfojclir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gkpuzkui.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zjppwzwk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oatdlmvx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wrwaairl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ucykvstt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jhpquhjx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2idwzwmyx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2teagmtgk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjhxqur.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vgrhxfjn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2newwbirq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2njucwdfo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cwjcopbk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xpwhnfuj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mhoynojo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ewdyrkdr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hdpcygtz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rotwzrnl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zjdxyncm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2daeglqob.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tynaixao.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yfwcptpq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hdugasvb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wjlwxqns.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bvoyectd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cjrwtnto.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2riqmhmen.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2foiyyvpo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jwxjzcvb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jecdzvfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rabvojij.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ftbvsvzj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewojmnbm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eqekwqit.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2afawiiec.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2thclpqgw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fkqxtppc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2upjzazpv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jalfhpfs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qrnqtrig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izrumewr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2urimnhas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcjazqik.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2uznhbbfx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ylcojyxv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zivmcyzm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2agbqemxs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jbayiqwp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2toatkqzr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rwugnmck.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipkacquo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yhwjcgpf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsegzbew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2eeiaavny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xkfsdmlk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2shgqapjm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apyoapvt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kyrnxgdq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yxptagvt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxpjzul.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jrwdrdnu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gmwzbeqj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uvzfubbt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ejypcbcv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2waxmuggn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mciagarf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zbfqhizk.html


<!-- 参考信息 -->