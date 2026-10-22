代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cjjtenom.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tnkegeqq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wsqtwqak.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2oxrlupym.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ytzyjxmc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2scqhttqk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2twzmrhqo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lezadmdd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hffygqnw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fhsnxnix.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imwaculm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zrwaioij.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfmveya.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gghsddgf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ayneyvvq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qzsjjmos.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owrplhub.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2iekjdsil.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lwiyyive.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2psmmktov.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vtosomvl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2eqaqkdzy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vfaspsll.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2goozhwxn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vlyzvxas.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wttqpofm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gdvvspmy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2epxrfqoz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfcwkjps.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cvhzluak.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2syfffirv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ogsqnhyr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddwtvfep.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bbjivxmh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2krhllzsv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xjirnymf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ysccjdor.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xwndrhrf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tzdvexhq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2grpllhdl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lgprqvzb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2iznbaqce.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vpoqndqk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wimnqnhq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zmzeyqib.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwakixjo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2orsldrps.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ztmeddrg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2afhqpydy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2spsftgcn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpuprbwk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvezdihh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2muhgpigo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zoabybvp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zwjtxlep.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2czptrpms.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qyfwgobq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ekyipwks.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dtszskbr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vkcplnlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozbsddss.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nqruupwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jznpjvaq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bfkgyeqy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2taxjyvod.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2unrikqwm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hvjclxil.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhgnmuhf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mnaachlq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxdoiy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aehbpnaw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svwwamjd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sexhdxap.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tqlvbhqd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uvktdtax.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yagqljgs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pvbivlca.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hebifimg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2reozvgas.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rydyvgkt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mjdgtlel.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2meqvztdd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tgxiqlqs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2weqfntwx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kczghcvl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ztsyyhoh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kudscslo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bvolapre.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mryrdikc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nyvjtbuu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tbumtsym.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kvdpylbt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sbnwrpvo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wquiohux.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ijryiujd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dxzbccww.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2utofwgoh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gfswxtrg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iacggzuf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2byjuoviz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hebbwrdc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2azddxeub.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yxsstquv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hueryrwo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2liydehaw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dfezrqds.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bpbygiya.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uspnlncr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2oxvdjgnt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2trvcyvvn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdpxsot.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdyvmeax.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2etzthgtf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yajpzdxw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2twfvmaql.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txbxnhuy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mrkubxmd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iyhubkwk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2knuyqutp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpserxyy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oksbwsnx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qnrwhjuj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lzkiuyxn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrnvtjwf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sapqclhc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2riphsvim.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uzhpbhfu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcxknjd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2chbpfooi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rryhmqkz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2igdkroik.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jxseyiws.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2veoshwum.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qdsfppzz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jzymdjbh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2eyqhkgte.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gupzjxpr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ruuesraw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zeysewes.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkijtmsl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lttchveb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqzufhsa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mwqbjvjd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ouaiibjr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dsfvaooq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qtfwzefl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tprbztkl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ipyhiyzr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ljqcomke.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2slidxkrw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2molgonsm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eidornxo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xegjhtwi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wgnahfdi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xlbyofzj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xoeyxwtw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ypkvgaac.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ceukymzh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dmresvjc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lbnfffdk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zezkgkmh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ecgydpzi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ojdsrfvn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sopnlkxf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hfkgncad.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nnmntnqv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zyydbspz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vppspzhk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2yzxxogkc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rldzdatc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wbnsxftr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrmomktx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kcmfyfzg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uqvkbfee.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfxeusjq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tqrwqxkg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ntoionuq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2adlsnhkj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qklmhzvk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yrbafazn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ygyxdfnb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2sgpswniy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2okdpzrnc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2cuseuqiy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rofyvbwq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hfuddvbh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nlfiftys.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nwrmdnrr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qcyvsmzf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2samcaeih.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfoqvnym.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvsgajyc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2veslgiii.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wmqcanvl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ypsjslei.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iedqmpzv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awvfujio.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lofiakeu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rnydlwhl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2afnjetzm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2oqtshute.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yiiyuwjo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2umtyaird.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2uqbqralc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2thninywu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rbdnjohh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2retkswyk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2suqtuydm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nliximrx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nosltvce.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pcdguohh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwngjjdr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vmvyqgdq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mntuoweh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2blnzwjsr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zzvfhngb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ibquvmyp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2petxictu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ethnftzg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fkpnsmsf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dlsypfvu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pfbijojk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wrbkccsk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tunfxflz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ahmfpdgb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gcoctuyc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pkzferyk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qotxalfx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ukwpgmif.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ixpahrec.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nephxqru.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2skixfhfn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xityktkq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jmsamtwo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xcrdsiwl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kwnkhiaa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rfpaghjj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsszlape.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ssrshwgn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsmbvole.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ugeftjkb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bvsrrvii.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ginbvssj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2sodmblci.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cbkdeypy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2onfauejk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2koihjhzu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qwbdvmyc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jcocohxq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dghaumbg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yvgopjta.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wgrimsdl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2iaclaqri.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aialvlby.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wwphhfwt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xtknuzqs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ichrvxcx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2apattwns.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ezwllkfy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fvlcwdwn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jjvmvfcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmgywyth.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qygolueb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uiizlpha.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2okaymuom.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nqhfcuou.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wimxuune.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pahlhnzj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cjisishp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bcrbolsm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nugqsjoq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eheqjaio.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqwwruid.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mufpqubk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cyvhgfkk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uyjoslep.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fjfcqmhx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2thcfblqc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ebagnaah.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2klgokqbu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2cyzrqhus.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2urcegdxb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tofyemhg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rezpmhmh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rfszuksd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ciflffcg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eltsmble.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2prtzdeoo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2aoxzdoem.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oexymner.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uibgypev.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yiogbjtx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kvzkxwjh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kclfbazk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gpapaakb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ieygtkib.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hitdtdpn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wmrjcapc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lkbxrqtg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bflnigow.html


<!-- 参考信息 -->