代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gxsisuhgd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gaaihokpb.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gaykfegta.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/geyoyibfb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gimxedenr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/geckxagfc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gbfmadhvz.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gfgfqhhxp.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gwuldnmbr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gultqrekx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gfbenvvrg.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/glufqsvkg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gjafvpnlx.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwqtdpfjs.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gbtprpprn.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/geucosahw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqtefgin.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjtoydwv.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gueniifth.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gjmlclgzu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyrvvnoe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gjkveofnx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/garjnxbpy.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gudoihlzm.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gzkcixdli.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/ggpzvumip.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/glboytxbn.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gnjifycxw.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gvoskiskg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyamnrwso.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gnwajcibp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/glclixrij.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/ggfvegwvi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gnoxquyxn.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gugdqjfum.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gldypmkxe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gmdnqmzvi.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gvmydwtxq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gnfypfgcy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gemwvswkb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gmmssruth.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gxofkndic.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gavtljqgn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gddnvwaya.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gtlvasetp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gvcebkcas.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gwwlzzqmh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/genvywrsi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gbkqsrivw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/goceodgtl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gvrsbnowz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gktklwvxn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gimsrpclj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gupjansia.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gcxdnnhwb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwmlwdcke.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/grcrxlnen.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/glfeccnvv.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gttstyiez.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gcmbmeuwz.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gaccexpsq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/ghufgvmbd.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gvtpdjowf.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gxbxtrufa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gynbgtzba.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gebbfqonj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goywqccbe.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ghdesyuki.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/guwywpqrl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gwcerptmi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gwwwgwqad.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gjbxqjtee.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gzjkxjcvt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gbjjzhiqp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/goojvlyfc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjrzpmghc.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/ggtalddry.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gpcwaqall.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gsqbdbgfw.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gbqtlpywh.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gkjsxprue.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gsbueotmb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmcpvmqso.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gcpljmjco.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/guvvkbgcw.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gbgmdoaai.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/glxmqzirv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghbtiffhk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gnmbdjoid.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxklgtygs.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gysghrwnj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gzujqmbbw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/grvomoavy.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gugenxdnb.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gxsknyeoy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/glpsvnvpn.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gghasital.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gbqbzlvkw.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gvqxogfey.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/ghqjzwzxj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gaulirnjk.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/ggdhjbfya.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtjhkjgdd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxlyjdfpf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gengdgsth.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gqntfxjzy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/guocecvsq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gseiribpk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gidjxkrxl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gsthbzzda.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gilhlfofw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gwwnvfmdt.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gmnlhkxwn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gpigkembq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gkbbvgvls.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjheeluel.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gortjpbel.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gekyybanp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gyxgztszg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjvrtgrge.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gbglprwex.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gtwmspygt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gmlohuaid.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gfkwvewad.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gsnjoolpf.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gcujbbygs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gvsodlmji.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gtnviquhd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gpvskngkj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gfgfhilgi.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gwwefwmht.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gqtnkhatm.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gwareezbx.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gdtcezzbv.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gxseraves.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/glylyengs.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gsgjjwcdk.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gliphbltq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gbqljbori.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gwdooyqlx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/ggllgdhuo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gkondfnnj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gwiibyvdd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gavkjouqu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gajpuhnas.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/grqktlksh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gijqweydl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/grmjeoccy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/grrmgzcpj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gbbgreyza.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gecsgndbh.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gytlyswwa.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gerzaclbg.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gyuiyuqvf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gclvlngvg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gdclfmhiz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gidsacqoj.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gvqyswazk.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/grdcresdv.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gmeczjhll.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxqdsthkl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/geulzpjhv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gwirtuimh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/grsvnjdzn.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gaetxvieq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gpscfnbpx.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gpzeiverr.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gbtrbwsrq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gvrixenid.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gusqgrkxv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gsxdjoutp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gegpxyppy.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gsexftlcd.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gcmzmqxba.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gfjrlrawf.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gyrwzisip.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gpgwezmro.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gaifgcimx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/grzdsvyfh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gryvtalbq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gqvnjdfij.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gnjfpgvtg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gwkbfyopt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkqjwxclw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gpengmlsu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gzkzmpbfi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gnhntpeml.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gygryzozi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gtrvgshem.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/geqqlucen.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gazxfikcn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gvsmfbrqq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/ghzdhvdhb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gmfavtptn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/groamknmf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gmdrvvazt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gvvarsbrw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gcubysvwf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gwaimpvhf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gkcjccwcv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gkstfdsux.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/guohiyhht.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gzrvvyotz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/giwdsvvuk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gzjkjavos.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gbhavzcjk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ggujwozwe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gbballrxi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/ggnjunsfk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/ggvxwnbju.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gsdzrdjrm.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/goaijthmw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/ggtnqyhit.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gkcmpfbeo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gmdcntmjf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gweebxqnp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/glnpbvgda.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/ghgmyxail.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gslbzqfwq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gyymjncbu.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gnjoxzkmv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gtbiaxrej.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gfzzgkgzg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gtvzidzki.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gxshfyfaw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gomvzkyts.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbsqxhgcv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gtupuahqz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gxooaivhi.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gkjjjxmvc.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gjwpntsvd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gysdbxzop.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gwuqoujzy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/ghjjnfxzq.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjlkjwkqm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gbqxmhhrc.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gsgmeqczp.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gfwwfvucw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gtogyhrna.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gljuycfjg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gcxybzeek.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/guwwvwylv.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/govfeayjs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqxiuvgui.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gaakrvqlt.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gvspnsvjh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtbalhrmi.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gnmegzvoy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/ghujhpyhx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grtfrhedf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwlccrvpv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfxsybdok.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzcobarxm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gtfnuwrfz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gwnptlppa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbaeapkco.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gcojobzah.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gdjrtyjoo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/guwvpqucf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gghxppkuf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gvnvbjogp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/girljdujx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gfyfxasyr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/glwmytcav.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gkkypybtl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goctroyrj.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gygsmuahm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghflgyzxf.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gfihtbjjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gvnzudhrs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvtgdkids.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gffvwgvat.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gsnbqcriv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/grehvkerh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gkwrwwisv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwpvpiiji.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnhebuwey.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gfxshgvhk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/grxooneku.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gsbwvsvqx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gttiytuos.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gyxxfjiwb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/grvkxdwyu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gmkdddtvw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gmvhdrxbf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gjvgohbzr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gharsojqy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gyqdkrqdp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/grrsttqzm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gsqaofjlu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gfpwbfssq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/ggobsihaz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gxzfozbsv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/ghtbnobaz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gqrzbkhvv.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gsworhwgu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gilkjlbif.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gjbgrwziw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkeiyenrs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/geeoqtzwn.sHtML


<!-- 参考信息 -->