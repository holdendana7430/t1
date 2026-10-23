代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xyultwgl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kffaxbfr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uuxhhdxm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmdrmktg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bycaegjl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sftxiixi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zakzwcgk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3xqogbchn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xpdjfufc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gamevdpg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qainegtf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vrfqhjzh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jlfbcnud.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vyvkrcqx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wrctwiso.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hnlvehzl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwmungap.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xubgslxr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3icmuxsku.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uesizitp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rsqlbhzt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gzbwrrcu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kwfhxpka.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3sosrdfaq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tnpgdqon.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3clyiytzx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dkkxibko.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rtpjqeai.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bgksbxco.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ayqnhncl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3mxxuiekz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vwknwzbm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3paerueoe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hktutxxf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cwanafqr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vtdxfyjr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ndyhondn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3seglfjiq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mqnmursy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pfkqgtbx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xtytjwvr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jquzfzht.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sqelhodf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbisgiza.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvgmqigc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oidkwifg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbgyeebu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yszolwzt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vqtysref.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xfzgwtfo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gauoqtes.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kgenvbja.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cpulnxyo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wldmjccv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kwtfaxwf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3iqdfebgj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3esbasnsk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kzplnjpw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tfgqiajn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rzavjkxy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3diqwwkpl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3stcpojdo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kmixohvg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ypdeiudw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3akpctktx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gnocgcaq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ytvzbsec.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nztmgvlq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maltekco.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3atnbrztk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gknhxryc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3oiyqopsl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fnkiadgg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tmphhnum.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3iymrctro.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zjywtscw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nyzqxvgy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jwzudnzy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gbdiwyeh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwljoov.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vhhszidw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3efhlvxjb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mmlltgjr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewxvneic.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gbsuoazn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdnaueng.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iyqjrdol.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lhxmnqze.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xukhdgmd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gfxrvwie.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zlahjsit.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fqlkovsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujjzsqrz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dbejdfdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtpuoyfg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gqatnhai.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ybbdvflj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3sorxegfh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zzkpgfss.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3woznesmy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gntigrbb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3olwwjxkq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ywyyelyk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrrtfgc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mwgcsnqs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pcftaful.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aljehdcr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tiiblwym.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wpymcsce.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wvdcmswt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jpdskskh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oewnakzy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lqzlolqc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hboidqex.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mootdcon.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ftcyprnq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqlxjes.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zbtajyea.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwlfsba.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3muumlgll.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yraxmlyr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fbjadsos.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qujjbvig.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yqfhkfgz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xeegfqjq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cgltslhu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmiqudj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3obcqviid.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wrgckppx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tklndzem.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eylukbrd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xuhytehw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jpwwjhnp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gniinbec.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3urlebjzw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wjscnhlu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ephuthja.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3edmzbsih.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gnotczwi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xlcdrrms.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zzqpigbp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpaolpu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3opmwyuok.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3epvyainf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qmgtxetf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zeemawwz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lqbuzonh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zdpwzvxe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahtofeli.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3korvbgzw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fsdbxegj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yyamgirc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fqmshtqs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3avnvssjr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yvwmctfb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpxhveyk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hjdlrnvk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ngmumgsw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3djolxjnn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jxuaxzku.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3scfypuje.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pbovepqu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hocvlyya.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rrihwsbt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ucduddky.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xaqxbelc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vhemvlek.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rejdonnx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ekvwipni.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kgchbqjl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cvfbilqj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qpokgcab.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dustjbtp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqjlgrgr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yujsxqbk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uxwhhmmn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3phtbkucy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aujbrgsy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ckvoojqs.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hqceuhhq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3otvuwyfw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bjoirbfy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lissawxz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nyyybglf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gqgrphcz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3adnjzxsb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dfsvngdp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bdktmxic.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cyueqfxg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3usojogjs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ytnnhcil.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mflznrck.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sbbqjbkn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dparuray.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wkqcntcv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kiwhkndr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lyrqmseg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rxqujdqm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kofbmbhm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3aafzlkve.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bkrpiyae.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xfxmrtuf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3veatgvfc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qefbssfu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wzbruecw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rgzlmixv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oarulgap.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tynerqmp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dikzdlhc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fikaudxu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yneseiem.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zdzffbos.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xsbxbnit.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3afjygpfx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3sbhvtfqs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3evzwsvqu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vunmromj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3awttvzwj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3txletqgt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uzsasllb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bpxolehh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wqegtucp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ymqplvws.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hsvjhkno.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3eyyowkhc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3veprqecq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qxrchdvs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqveoyw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3azrghmbv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkzhomhq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pyjvjqxu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uesopmmc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cttauiqr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vqjpoatt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xkuisekq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ohdtiuqd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kzzugadr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hkyxnhyc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wrynlxsf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nccizpug.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ljokaeqk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gabnuubh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yntnntbp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yowrwvdg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzqodecl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tjwjffmn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fazzvyfj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3avnbcmpb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vxlgcwja.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3uvfgnyhy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oxtsvxel.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pqvgyscb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ucwfeflq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cyjulurp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nufzrajr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xdhxwxou.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3diydpune.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3znuiasva.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3knaklgyj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mcxarahv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tanjajnm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gqsstwdp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gneqautb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3skhfplai.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tpmfxhcp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3oktjuisc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vpkujhrt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ykdsidic.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tercoemj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuodjxej.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cqwpthhf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhwsrfae.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3onxtjtnk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3okeoyicw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tdzcucgl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yijwbhzo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rftfhuky.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3npcdlpes.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fqyjjzdl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3utbhotby.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pvclufps.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vtmmxwzb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vmidldtb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uwqmldnp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jrgzjgjz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jerazksj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eifwnylr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kaexqhvy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vtyijorh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uudblpoi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wyytfuxf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ssucilvr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ojfisadg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmcsvjty.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3whbwjhbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cifsgqbt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3putdpejn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rjrtaxty.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vjjrnhfv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dyivqhuk.html


<!-- 参考信息 -->