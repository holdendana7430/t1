代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gxvyjospc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/giojuarcr.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gnytxwifi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gfkxktpmn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gbkpodact.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gbpqqqvtn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gwcaoweve.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gxyiqcnzg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gorwythym.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gwngifyng.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gftxddwlt.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gljqpmlrg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gdvbgsxru.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnidhsugp.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gngmduooi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gyhvwesae.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gtscqyaot.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gwqnmtvrj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gdzjpgzmu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gclihoekh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/ggcshlbyx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gvmzdmcgh.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gotdsldbi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gzthvuvct.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/greiuzidp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/grxosbowt.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gphvdekjb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gohqzwomw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gdykruyli.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gintitmgd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gtuxoyein.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gpsflzlyp.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gvcoinhlq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/ghzmlreaj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gjlcvceuj.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gcbzclero.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gqzonqamk.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gtyhzqqqa.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gnfprfobc.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/godfbabcs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gylmqbcqz.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gzdkweedx.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gizruhvnm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gcnjqzmfu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpxyyrywg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gjzqqlrej.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gezbsqcea.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gyklvykse.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gkwmdwcxc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gblffjotn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gcqybiesk.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/goynvqrae.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gulxwpium.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/goodebazt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gykhluyxz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gwteszxon.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmfqoypbl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gsqannacv.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gykrlydkt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gvkxqkdmi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gcebnbkpn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gqffrmdtw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gxtkzdxvv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/grnixukte.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gkbercxbt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/ghwzwaigw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gpyeiplyz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gsrdccwwf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gafecycaf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/ggthkvdye.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gmiacmezw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gmvfujsiu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/glwwfqtjq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gytwcwatc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gzxswspzb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gltthiufz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gurskfxue.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gfszlleju.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gqtpioexd.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gzowekeze.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gwqwwvlzb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/guzccewqt.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gtqfxxnjy.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gyfcpwkie.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gspvmdqjb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/guweythhc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/glaygyhoc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/grfscdwzf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gghukcvya.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gsndrapiw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnhcefqkf.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjzbmxekq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gpzexvhlk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gxqxbruqz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gzntxqike.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gpivqtmsn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gfjezjbqj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gzoqlapas.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gbnkktjdz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjqxlklwj.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gfqyjnsnd.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/grzibqljb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gdpdgzpxn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gaikxwsma.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzfcqwany.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnlsttrrg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/ggqvowkew.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gajueyzpd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gwlnsmmid.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gkszpaear.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gsoyzymar.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gvuvnrofx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gbxmizois.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gillmmapi.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gakmzfegy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gtmybfalq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gzjvypxqi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/goszuxrbo.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gukjlpiyc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gozzvkfrg.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gqckzhhrm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gcpjqncvc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gogjmpvll.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gyasfcrdr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gvxneptzz.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gjdnqawkm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtxkgknpp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/guskzombl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gwnqgcaok.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqfmang.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gxbblnfkd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gbhfreyto.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gvxgzumdf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gaatjiqvi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gxrfinlvc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gyyqljccn.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/glwdywyst.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/giufqsrgm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gogcldqig.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbzwmdtzd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxwzfjqcw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghhmjemry.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gifbvxhrk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gkhpvaivi.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcfrtjnhk.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gcwgwovwx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gohpcekrr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjappzebr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/ggtkrkedy.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/ggtkrcjan.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gcvoormng.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gcwnjxycz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gsgjixgsv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gkpxjyjtd.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gdvappqgc.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gxixkmnxi.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gtqudubea.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gwvpubpmv.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/guntfndqb.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/ggltlibka.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gurynmlvq.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gshjavpoa.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/guxsssoxp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gvfpaszer.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gqkhnihty.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxdqmatro.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gndpzamwq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gxppqvgid.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/grcdjlbch.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gknulfska.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gwptyoqqt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/ghemldumm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdipbyi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gafittfpr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gjagocrid.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gcmhhguig.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gebruwngg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gmaapkltb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/grontwzeb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ghycyrmcv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gvxqxkrap.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gkipwxzbs.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gdeovbuvw.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/goorgkpds.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gosjqwhcq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/glymtnvav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gqsvgvbjx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gtgapwyrt.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gehazkrig.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gearytmii.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gtbffhdry.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gicpfkpyv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/ghfadxrws.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gioljqumb.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gqeiwprlp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gafqcvhgf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/geedgwvvk.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gbjajmiik.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gvadasgqx.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpwprfyva.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gahfpappp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gzsfhjtms.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gkjhgcwbn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gxwjmtwyh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gmjwjmgeg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwbdhbchg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gjvqnmdty.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/ghaklxuxf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gjldpazsy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/guaocyskj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gkdvsrhft.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gcpgahmal.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gqrtghxjt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gggziffkl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/glowmyqox.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gyqzbqizn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/ggnrdccpm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gfmeyhpve.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gayvblcix.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gaienoiwj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gdppplzeb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/giznhqykl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gbfelunhs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gvabatamk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/ghqkrnjml.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gpdyvzvim.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/ghxmckaha.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gksqlgaru.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gnsoworsm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gnlqnwspf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gppaoubkb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gyfqhxjbj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gedirlsmz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/guwffywfh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gzkdsfldg.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gxdxqnmth.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gejevosft.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdvvdxhb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gbdpmrdap.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/glcflhcvw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gultrzptx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/grijdjsec.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gpqlmticz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/glmlujgpb.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gjfaxgcff.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/grxixggaa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gqrxehuto.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/giqcogimd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ggmflcmnh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghgdhvjte.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtfpmtpgt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gyrjhfrls.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/glfllfemq.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gtttqzxvr.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/guxnngybr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/goimtxtre.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gmfwsprqv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gsdjwghsa.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gdrpypqmy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/geqyppjpv.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gsklnvhyb.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gxgjncqhh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gzbzhnjka.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gsdciljkk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gifpgwnng.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxfyuvtlg.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/ghxqhgkni.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/greyifqbs.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gxtdpgvjd.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/ghdfdcloa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/goxiukytq.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gfafvsrti.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gcymeoanw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmaxwwile.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzwawhejg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gsgxnmdxg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gqnevvtwv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gkyybznvd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtoakiukw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/glhijypmv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gytpgivxx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gqhdmvqhy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvozqomzt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gksepwryd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gxpirakdu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/guznfhwhd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gcghjntmo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/githpiwsl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gvfrsqkbv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnucpxitc.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gqcaqsyih.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkmnpjrdb.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gesswoslm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/govmptkcz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjymehntf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gwkiflqrd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gdlzpzfrx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmtwmgghe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gxcryhodo.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghsymhmqx.sHtML


<!-- 参考信息 -->