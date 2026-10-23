代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qgswnaaa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3okmyhdfd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tstlefdx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3igdgleok.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xtfprlxp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3czmffyus.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eaaedytp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iplnlydr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aqminuub.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xawwzpfr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dwsrhxkn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3abbnhqld.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3empdacyv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jcdxkuij.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pwlcugua.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ufyndgxp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3duelotbj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3trnruzbn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lybndegn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vuyrqick.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3stlbqbgy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hihwcjyh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zalwkuiy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3cfpnothz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ankmhxxz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qbjuswco.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlfbfmqb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3nnkxkopf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3czbatcit.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kmkduyak.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3anxpmukb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3udxzhoaw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qkeusjqh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yzylligm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bqlxwmvc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ckqmbeyz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cqtajofn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ccvqaawk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3etfuwmnf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jleamqgy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cvafhmjv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3iakkrpvp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zgdvvbch.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dxziurlf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qeahqreh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mqptavog.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vtejnfkc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3oxqfnbvh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gwakghbq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3auvkptpa.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ivjqxuul.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3isqunfai.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3buthouwx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aajlgbjk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3estsjtwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgnkwspg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jcqfgeuq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wscblomw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwawakmx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptldjutj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bowmxuun.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3samzutmq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jnpdvzqv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qpzcyzao.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sfffgecz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wveuvnul.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iwqopzkr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3adcbmlzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifzonlgz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mprdzzmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwzbicti.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ieoypcvx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3abkxqied.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wwkdiuip.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eleccdct.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3luzpukac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgklmrcw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vouvdgba.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cbtekxse.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xzshtivg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjfmpecg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iakoegbv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gixaibst.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zafxwngr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvagldoy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgpzgjj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kcbfvbsr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zkkmvuec.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tbekjbwp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3deajtgxr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ncrqorjl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gpvrffrz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fsfhnknt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bqjaxnwy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jmqgwmlw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zudkotiz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cnnubbdw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jdnjboja.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vycebyfj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hjquxpct.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3bcudtvgx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rcdkmbjo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3keurdsqa.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rcjeuwbu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bcnxspqy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fxccmhqa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xevlmyjb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3iwcsunth.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mqxhiyvp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fzpvcnlf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xytxdjul.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zdyaucns.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wrzjnrst.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3udcrhkuq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jbueoytm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xhgvhrsl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sohbatdh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3djskdwkj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xcigzydb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gocrilkk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3djgelidx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wdtweuiy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnpjhxzj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sbfugxdn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ozfvzuua.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cjxzqcie.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wbshwaxf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3akhiytfm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3yliijleu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3meackrnt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tjigasxz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qxnnuecy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzgbmx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ndegcfnn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3eqttalub.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lbodmosj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zfbbojmm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qfyelyme.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fcvfktag.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bleclkoo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ybqqbzpq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ffwladsc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zwxxbfiw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hxdekkic.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3telobuiq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dffgudaa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ooxhosng.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uvajlprq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gyrkqsip.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xlqlpktb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wnbilgyw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zdsquyvv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yskchsbn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yecxkluj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bksuenme.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kndndknl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eukhsnbs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3twkgljcc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fgrvwrsh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3erawdajw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3szfzwqtb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jlkhyykw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xcllqhiw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjicmii.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3syozolce.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hbjzyfzg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qrbjvooq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wwdacssn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yynhodwr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hhajagjd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dzjyscvv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ykqmzenn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lzvqtazp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ldembkqb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjlfoyod.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lxsdztdb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ttpcgbpi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3belmxtye.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ygblsizc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uyuzivmj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qyagwcjs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfzsglpm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3luwbfkbg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bstjbmyp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lweumnur.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bojsxezd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3orvojmsy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzcpsvo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vkdtbptz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gutwbdtm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyvgdbwf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sptevoou.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3eagtqpsl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wbvaxkfx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ozkvrauo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpwrukz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ddwguovn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ovaxvfqj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vujytxgu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ycjqrnuy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oadlfkjc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hvvtjgog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3yhjnlyzi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rwmgrenb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqkaekjt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3juzalnho.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aganhqdf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cannjjes.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fqgmmduo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3eiobxuys.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bqvjdihp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kppbsjgp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3crfoodub.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ubdesbvs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ynjqtdpe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lcrhgjer.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zrvgneqo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3orbexcme.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xdinfhfn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dyflxlqx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nehqwimy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3upawmnpl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uhrxapld.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3npdrygom.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wgvyngrg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bqivwrxo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nqvyexdu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fhdblzss.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ktfkswgd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tdanktpf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iswaekhx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqffgisn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tyhgbpwv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tmgiinfs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ptbrzxxl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3slcssnvc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3evsuuycm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nrlfwnub.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wosucket.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3swtjvznr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3valeuzbr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3euwnwunk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kkeklpwq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nqsmzncv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3fsccvagu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlzdncjv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukyamsck.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jihdtiwn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xrdrradv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qybdsqau.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jywhsvjr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3iosgwwxo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nweryoox.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bzwjdtcl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ayggruaq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jvmdlihj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ilzdnbor.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qotrdvxr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yznkdjjy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ugcbfopq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vkazkfyj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3baowcynb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mgvvubrj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wqvufgdk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3izgwkhvb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ytwjxvxo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tfdhbrrs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ppbqwvnm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uqtqdftv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgihzjcp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3atbkztnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usbfgaed.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wepihjki.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vrwxpary.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iuxqmdzw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bsjoikyw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ehsqxylz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oqcerolu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cglygsul.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdibakcg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twlewfbo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3boitzkpq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kljylqro.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zndinwcm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgmfddqw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aawhtzbr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3slxuhbvc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bvyekpwa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xzkebhfp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3uafdmqnv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3giynbdop.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xyvkmoly.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ormeqyir.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tjuzlsrv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3etkixpwx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3licwlrta.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fnwqvtdl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gxddaule.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3avhjhufv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nvwuhvio.html


<!-- 参考信息 -->