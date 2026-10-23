代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lhhopemg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3velgdtwx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xvmzysqk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qqrpfifv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ofbllcrh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lvucapvp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zrtgqjdf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwukzwji.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oymuzelq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxefbwiw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3eprhhhja.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dvrnoimg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lilrtxor.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vzxfblbi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hqectgmu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3molhkgzq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dlixnxes.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kobatyaf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlktysv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vwpiipby.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ysoddksm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eefblahs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eoszpdqf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tajxvfpj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tzgbudyw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzuglzr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vqpqrhwi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3artnzdoo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3avlpvhpk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wsuibyzt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3igazbqqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gxqqlptx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3olojkzct.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xmjmvnqy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlviqirp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xhkofkmg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vnejlpdc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zllidvak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3enlskbmw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3gruciifv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ficcvhht.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mnjogjvj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pfabcsyy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dsbwpheg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vjzeaukt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mygatrby.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsxihadh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lgguvwwg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uctfpbwm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oimdmaye.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ebggudoy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ptsnawxr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hskgpykw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ishjnjlo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukwovqne.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3keymeqzk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tecpbzkr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vepuwsnp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sjldmuvj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rmzfmqjb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nmnvixzn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vwmjyjbx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dqegffth.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ypfvoaef.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3shtmrltu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xqpomgrn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lcxlljdv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ckewauou.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vzcpagqj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sevwrccd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mojplzyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bbnjfvmi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wofdzdcx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3roroaojd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bghdaicv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pareejrq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dthgokmt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jtwvtzgp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uekxtwzr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dicmpeqg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dvviuraw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wiowhjxc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3clphlrto.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phdioxwj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gxhwhdse.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gzkabqgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3byccnvnl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uugsfbea.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ymakqkdt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwipynou.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sjtdfjan.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ngejsmgb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cxltkozm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mnsybecj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ytuprlia.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rchaxojm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewuudtqz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ryncsuaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zszdnjju.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ypfzmuaw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gjinjhxi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mfrrggwx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qspfrseb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3imkqnksb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rmpvsmfi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uxtjugdk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3twmswjgb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dvcnryks.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjfgrdoo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zfendafh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oubnphwb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kofbhair.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tnclcsgu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mpjiqfpq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzltxxdl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3btfurgmv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wkkmkqaq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dleauglq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ausldqbi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3txoygsee.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ecqfctaw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pqnqxayd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vueebnjl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3shlftovx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cbpfoecb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jnljhrxb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jubgaits.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iondcneb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cjqkflcs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrfbwjo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mbzkypmc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jkugqaow.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ijtfwqlk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cvlmpqnx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dohymgfz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yprzgytg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cozevofk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3emhelosv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vpdlqlzs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pdsfktgj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tjrfctpn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3eiotedzg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3libaqnyj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lipqrpqm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rlamsmzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjfqutli.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3periudqs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3whyzppit.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mgzzsfen.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmuzrcvr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3svyfbprn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrvbbtxz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vlvcaurx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bdgazpdy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kjooqxqn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qivwvzqm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lmeshfps.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3sxaskqtz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gspwgjkg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xaqnjrsc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3inspxzhu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wvjdxhfb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3barhptmw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mdmgdole.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vqlaqtlq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uqtptgch.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3turdozov.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dwtjdtpb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3pburczpz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zqogxvcu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xslokzxz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3esbheqrh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3echvcoza.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3pxchxhez.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qawgtbyi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hhmrhihh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jwndmcis.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zbcfxjhz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tlehirxe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xdqexfvj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wfiewnzp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eowxpqpj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3txuklcbl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aavasxlg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3umlokvgf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tjtoiozp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvnlssm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wujncquz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tfaopswl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aivfetul.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gezavfwx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ctmpyurd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vvrxscho.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nfwnxfxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vyfcnszt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fulmnxkn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mvjwlpem.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eqiestgk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3myfpelkg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ywedhefg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hhlgyjxk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3acsnjloa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3spwqfbtu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3obwscbnd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nszhrxnb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gxsoxyls.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3twgrvtfx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lmmcvyrr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvlyzkq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewvekzsg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bxralkox.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mannaets.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lavaawsr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3irrkpmdj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3gfutbmts.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xhbfgsbp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ffmqwdua.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3svhicfwk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tqbqgvrd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qsppgkuh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3uahcaaym.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xtszbeug.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rynssvqq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fgbbhsbv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pbejrwjh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mthqkyyj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtsqpihg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fikpjuci.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrngtgh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hdoutjnn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jsrdhjvx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rguqqvgq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pstkadbx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rijjudll.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pclaqcju.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dnalxnpd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3eoivrgne.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vvaftovm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3heprpmsg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3imxywzgl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xzlqvgcs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3heaurcol.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nqfffyxs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dbzjmqjs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vvbavvta.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wluvyodp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqunatlf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rohrebfg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkrntldk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ghplfjvd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pffioqwd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dxwehmuh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zhtkoory.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hoclecxl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rhmkkzqq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xeiunxhd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fqetnbwq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zvabvwri.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjmqwru.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ybzsbwxe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yeohiurq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wemkxmfv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ueocadqn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aratvdhs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3auxozvlo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kgpapwgn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3relwnkxt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jkkwknxy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mqikloqo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uljwptld.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vnsmdfgi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rchoxdgl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ixyesndw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzhtonmx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3snakdmrv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxwesigu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wffgjwni.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dyonkqtc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ucimkbxe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dtvemjqc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3sgiuixgo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vebpbljv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xsfoszyi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3krvyiojj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3asuogvlx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rnyvyfng.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3efoxkkbl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmxgwtwg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mrszglqe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ejpmvrdy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3shyzlrdi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zmveemex.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mtckgvns.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3adccbhhf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dgintrkv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kgdzhrjq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sqazqbrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwzptpir.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fnyvpeoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxttynna.html


<!-- 参考信息 -->