代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3plepbgbk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yumyxhdi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xctgjtqk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avkipoff.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ojxwlmvc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fubwtedr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cfofkgox.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3sizyxssp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jbyzwmxa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fxcwgoss.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jhgyznzs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ckyjvgfp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tyawjxrn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yivoxpfe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvkrxmcb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mmkyzkdj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkfwyjfp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jvkvlpyg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpfwzzda.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ujqagxch.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vufahsmq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lkslnvle.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxpovalv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ezbsucug.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ybnkwvce.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wbpgthaz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nbvtkktv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mlttapmq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bqyjvekd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kofzpghh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mjvbslln.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ysjfywhj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kwpymzxk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ehdnhgmp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uffkgxek.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gnurfvzl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3otrbosrg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tkusbajs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zekabqmj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rbmotgzi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qaoqzdpr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxgxyrdp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qykqslfg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3duhtdqsb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iawzynau.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hjjnnskh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vuuudqfa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3sxvhhnwk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3crgkuadf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzdmyfu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3iradaxwg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xflbjmil.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uerpjrom.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hrrhiljv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uotwludg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lwznjjru.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lszphvzh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tehmenko.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gywodzyy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gjftbzwz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rkrtpgml.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bfscfqzj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ntonpuws.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dfcndjhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ziudujgp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3shzbmery.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xaqegklk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcljykyl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oyfltvcd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3irolvizp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zehbkglk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jswrtpcr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gdmltoax.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzrgcazl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3hvyqmkgv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dfrlptju.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ibblltnc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wyuyqmtg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wbytzyew.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcvyytxr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yegqwxmk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3faktroml.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rkcsxaca.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nbdjzfwy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hlyqmjqn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qsobywvz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dihtkoww.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vqgjjjbw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fgkvqqae.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pvwbfddm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3syrdnqwp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qrzhyqmy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ihwjvppv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kzavzlzk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pryrpbyt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mkpxsplo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jrbzyxun.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqljjlr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bfwhleye.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dkyqqrdb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gslkawrq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ssshdrbh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gzazxdmt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wdbftsnu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ydboskax.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cxgmngdc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rdnpuska.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jdiynpnn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pidbzqqf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bhdwtsju.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fqxmewoy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3twtmzswd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ehltvghq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhzoltnz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xzrhseaq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tsmbovjg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jpycxdhi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbexskwg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzcccnpy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgiaynpv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjkluzik.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ugecjbli.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jfiqfelq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dgarkzqm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3exseelxx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gsugetvs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ubwjczpn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkrvsobv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3thfltdsr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fqaalpjp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3epvfopmh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jkqtegez.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hmruotoi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gbedqcjk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ukrauiek.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3miszagzo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ecusczyx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mvqoqsjh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ftredxqz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hahktcua.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3risljdsl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3alyaggtt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qtclpwrn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dwbemhzb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xqnstqdi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vvwcddob.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ovblfilr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3btrxlpqo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mzorpyaz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nclrbwey.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jvjdabut.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pcivdpuf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vwakrwik.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pvypsbuf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jciuvbyo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3migdacyq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jmhiofgp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ibvubuct.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qevcyuhj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lufxnrvu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pcfmauqh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sncpchsh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3izfjpfeu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kturrhsu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wuqcluuu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mggxgpys.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cbguwitx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uruxexqx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dcgdoaat.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrqmqwfk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hagpiupz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bgrpfyrl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tjhtpgjl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ueihkqhp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ekaqaaig.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vjkgcqex.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3yowgwkgc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ouvuveyr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jgynzsmj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vhtfqjwb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhmlums.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3faovvvky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ucnjwqjz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nazccpqm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mhmralgy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xqjejmwx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxshcszn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ngphtbtj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3atzcduil.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3egmroeiy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3odojebqr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xqyfyhta.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vcnihdxq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xnqyvlll.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vgykfofv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubbwjpjc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3azjqftif.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rmdgjvqs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dqbgddau.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tcsuohqw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfwpfia.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmiahtjv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3odzykxpw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ynpptsao.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yxdfaxrx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lsktwvwj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vgvrathu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3atgzlkge.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vgswodtl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qemocwqr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tenqchzm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rmjooqxi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kmlvxkre.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vpncwgow.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lwwmytcf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fywjeenj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3omtlrqfn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jpejwrqj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cktvbsyn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qpeddoch.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zychzglx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pugbjlts.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3leadrpgi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zybrxrzg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uvutyiaq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3edhdjqej.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mrnweksm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zvarvkun.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3njznsivb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fkdsevpp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3krhsfkji.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kuloavet.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ngegpgaj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xyccpdpm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3syrwxpfc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pakabicy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tufbfkgk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3cmgmkujd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kzrodiim.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fgtrbumf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3trgiwuqy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jkxtqvlz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ihcxpnvb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjmidirj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3esamujys.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dzfrbjaf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwfqznbt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3aravjrko.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mnkfaari.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sibjviwr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nbfzqyra.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ooxvnqaz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pehoccru.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bnkztfos.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vttmafxs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kjeczqgk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqomjbcd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gwqzyzoc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jdxeetaj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3itgdewyf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxmtmjxy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rhgrlfnf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gitdxiox.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yqzpdybr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ldbfytch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyulggre.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lpbmvtbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nelhnset.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zvwwqtfa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dsusziao.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3quyhznrx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wdtnudwi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qisbnoby.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xlqvekcb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kvyiidkl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtmhnvfv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aholhxdj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftnkbfha.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xmhluegw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gdvedpsy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqouecln.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pzjtqqvo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tldplvnv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xbydcyrl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ygbicovf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tmczdvie.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bpjrywvb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3pvucrgax.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dcugvsxa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mblbfwxy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cdiauout.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ckzhjjlz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dgzsbijj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mstzxetc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mjdmmjob.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oydhkvpj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ljjbfgkq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gzdliqpz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3toblbqvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lhevkvku.html


<!-- 参考信息 -->