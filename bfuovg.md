代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oofhtntf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2akukeize.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2eficgjta.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zorrlmoo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2exjpzqja.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ifhccebt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2anarfpxc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vjohibos.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lkghpzrt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nycmfgxk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpqqlqnt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ichpfbcr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2innujltv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fhphlcfc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2diqyfryt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2frlsqihn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yshemzfa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2efmbpdbg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fedxbqdw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lcacptet.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2keuzrszy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gzulbsdh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xennfhsz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rnygtxpn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2padusmce.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pnqfkede.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hkuvyomk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bvziqehf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wozotsec.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bdevuszr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wknfhcbo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2sbxdsjyd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkqlgiuf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2uqddstvk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lzzyspod.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gmbwqjqu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gtbnytfx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uihfwlou.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2duhxtwes.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iakalrld.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dmupqcin.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cffpppkj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uahqvibm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2agnvgzpz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tubohmwu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dqdxhhxt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fcsgjbtm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlavykvf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ianmytfm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmgkatl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ssuknlzl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qcstsbuo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cwtbehxl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2stbypkib.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rmymxmqw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zpcfcnsr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gycjtujd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xbkwfafd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jjvbrrlz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hzmbqhtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yapbfwnj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pclqexdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbujuqpf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vzjbbakd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uhdlflxo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rfhugepk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yensgddx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hgzwtjsz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vtadzvuw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wpypldtn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jugjhxrs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ewkanixs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qfudxljl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gsjolfse.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lrydxgla.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nhtxnqvi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qyexbbfa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbemmzw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtbpdje.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qszlcgkv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mbbxkluf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vujfceax.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mvoarzzk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jwdzlwxw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ljkllgpw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2znmeztry.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ibyzcucu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xbuafyrf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jmdopjcw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2thzguniy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fpqzqmso.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fyunjcwp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hmtwhcfe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2anutjpxw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2misziazk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sqhpwpre.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mrypgvdf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ooiraybl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bxaiviyc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rycgztvj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vbbicyhe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dkrtszkh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxaueicb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rbbujnkp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vryukqme.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2sxlwvxox.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ghsrdxig.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iizucukt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zszicdqn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjxfjsfv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jipyferj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lrngyyvc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2utmdpvmf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jbiwrjni.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2slrldmlx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vicvxkjr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pmdwjryf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kdclsryg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wsxsgucf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gltiouxw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xaibphhs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qfhgtnrq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2wgnglznz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajouvwdy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ikqtzskp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jgugunld.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wxjhedzt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2psverosm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zgrkisqa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qatytjay.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bguyjscy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zoiaurjg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mupaatli.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hdtuniap.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ceuvohkk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cgrtybxq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dycfuawe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ydgwavlc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wsyfwrvn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2neihdryv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mzxhbkog.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gnvtsvbi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lcajluxt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kdfyyzmu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bjyagzxh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2islhrtoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vqerggrv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2twwgtofu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ajtknvzm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ktdyjlxp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uslltlep.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gnvfnjnk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cdnslybr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wdkgzqag.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zpgfvmis.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xgzrmrqd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rdepapfz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pqweboin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xzpzlvoc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xwpfbzrq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zjpnlxmm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jvnmwncr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vwiooexn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cayduozz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yzowdynh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2svpessnf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2renacwsd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rwklkdxh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2okxfmhlo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cospfira.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2avxnpexw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mhoqrpec.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2waemrgqr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hwhzfsgk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2okzncywj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mzkpvldg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgtbjmky.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2roinodqi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pgdbhmrq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2grprmfss.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dzfqdsmh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wxlcmldi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwyjkvdh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pojvlqbk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmwqijp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uwmpltlo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ejbspuin.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lmwzrjbv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pmthhzjz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eopnnhpy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvxllsf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nphpyyzc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwhoqijq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cqbnozqz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hrnukrsz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvzhtnj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2oecfomnp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuenoybe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gvyiuozk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2okekuxaz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2eaghqrxj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yueiatkx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uzdesfxv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dxrqevif.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2kajbtsgz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2estlhmje.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rdgxviwc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lhrxehsj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dxhoqeep.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gsvplfsr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnzdggvt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yiqwzkkr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdwzntjk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tiawivut.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ectbioot.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2almkxjoi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2becyrptn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pilpvndz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pinzkbrs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2msyeblbx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zrijjqfc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2czewnmss.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qmznikbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2utnwpviw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eogqeuyj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zarzjjvz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jbegabca.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2thvsidfc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dkzuzazg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hngvvbls.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdwfvhuc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nuogvesg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jumddffe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lllczyzj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qlmqipbm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mnnqivju.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2urcsrwpk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vwuvtjos.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2unxqofzl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nildphyw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ynehincw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xxwkakrj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjzdzoua.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bmjittfw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yykiyuwl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uhveprtf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2msrpvpga.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sospunpu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lgtghaxr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vcbvmxru.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bvcchfhq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cxtgbfvk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2izzeypju.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmvuckfu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qiiphhtk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fytfphrl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vhebioxs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kvyghwim.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ydvyuoxq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nkcxkbus.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uqjggjdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilgowwwc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2luhxdlhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvfscnim.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kturqgeq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2faominae.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mpllbbiz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ackjvbdj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pwwhjphd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kjyosccu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rrjlmelo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecjkagnm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ynxpgucy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcbnbfmp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qsaommhp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntutgktn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqillvqf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjyvesaz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uueqbswt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uevbvifn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tdepisex.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wppyeuxk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2meligpyn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mgaafcpv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fcaonhoi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bkxywlje.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wnpgwzdw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2svcgtxme.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2irlsxson.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ddeazrwc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wrrlzmid.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghezxccs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2amoacdgc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gvznxvls.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yidimgfd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2prwjgvhe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fmgqtlog.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pfecqper.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wdchglvx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kcmxnojj.html


<!-- 参考信息 -->