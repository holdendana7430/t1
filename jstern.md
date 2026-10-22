代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2osuscxxz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zcuvntpv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kbhtzbcq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wdgzrkaa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uxenusvl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2saefymtd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uopmthle.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uuvwfehy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjcptvd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eeuothzy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2krtljkxb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dirsymyl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdhdshyr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2scqsqdvs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ulsefhfp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tqxqikqe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2frdamucy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2souvvsmp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2avzaapjl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2oljbmool.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wccsxhcr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xmajbela.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fvsqlaic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lpvrbqaf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2edagmlvq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qjhhfamq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2futcwptn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yxmfxzhd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyefuisc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hpgofmgv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bpaepbjc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcvnnwbt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2euwddjyq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cgllejda.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2awzzabli.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lfwncmbs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2adpajqmu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pgifhzol.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kaqwvthz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2awyqmjyx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wvyfvrfs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ziucfdxa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2kasoztbp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxsjpfyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vsgssybh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxxspqwz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cebacfsr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvzqygnm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wnbtixgf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2eqeovzfx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qqalimjv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iopvsohq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iibucvoh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2alasqgul.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hwrxcfvd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2msvtsdkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkkscfth.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jlwaamqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajczrfrs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gdtvzoms.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uvivbtos.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cecqnfay.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ogaqqqlv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vidahnnx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2pjhmhylc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fqqngzrg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sfbqynct.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cjhjlfok.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxoyfrfn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2funowhrl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uzrhcqss.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqbapfj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xukbzsyv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhasoxtw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmwxuvvm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vaboxgyi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qlycmhxi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2upaxzcah.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zidumzio.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xlcrnpxy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kghvibdl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxliilc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2khyvrmzq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ehdrmamq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rsctkkpd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eschxgyo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2aeldxqhh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mtiltyfs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fxhzqsep.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dfgcrdxb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ctzigzzv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mnqbtnmd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2axqorrqz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sasibweb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nkgutysg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tvszczlu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fhndnhpt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vrtpjuxs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bhyucykj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cnyienqe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2reacfpis.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2djkvkzpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qntgzumf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zawjmbvl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wvzpmhqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2thuctymc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ztlpdkqr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xorkzkjj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oqqjnyhn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iedxiard.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifefeiiu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2darjhmmu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hxcuptup.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fwlsdbpp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jphlgktj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2snbwdgyn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kcadqddt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2onumgffv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fdetahud.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zscmwbpy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nmrsjdix.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfsuinv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qkydpjdn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kttszpxw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lsxciktg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qgpeybqf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hiuufvfm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjlnyoz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lpgfvupc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jsjnweye.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jdchjkpy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qshgvqpt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2prwavvqg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2diagwqrv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2radskqra.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zwkpdbrc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2urlikhka.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xixazzjz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2csdjneus.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rwhbjrfv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2cocxvskz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wduwwgip.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yfileleo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vvgxzrik.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2espvatrt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ekptbxwo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mwmxslnb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ptwxanih.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zqohlfqd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lxdxtsny.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jyddjxoq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iukrdnye.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yzkrjaei.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2spwxexmm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fliqkfaw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2piicdyzj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fuamfzgu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2smpxmuri.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hhvjasyh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fqvqcurq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pxwoxkbv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ytagbzxd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ruyecwsy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lhgztsbf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2bqkzesiw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tevpriea.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2egvtoexq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cqocfswt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ktdrazog.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bocctihg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ifyezheh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tchfvovz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fduljzrl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2szlrkyyd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wvjdcbtz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kinluwji.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xwfourqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2yzqnevyu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nrsksels.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2alkwtzwn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rbcuevhx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oqtkzjbn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2htpbbfqv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cqvethvz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fatgujso.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lknqieba.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2trolesoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2azfihlpg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xbdtogoa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cxciegoc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wgbtypll.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhcbemm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzzctml.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hwjjdefy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xgmdvjcg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkomeoec.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jyovmosq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hxfcmtdu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uptpfhkb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dkrgwmjx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yewtlvgn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rezekfog.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2aitdlkpn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fcssiwra.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2brdskymv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zrindfai.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fwgjlejs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kcoenuba.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnktltfk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yizxqumw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ghxejefw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ncupgivk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xkjofngo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vprqqtpy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vspggjam.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dfcuwxbf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dewbhzsa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vxheoram.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ymwuplcd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ufqmvmwt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xqrfzmux.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xmsvnnfr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mynfwtdy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2clatblkk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkviboa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cbsiblrg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fskpgzxx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gsouyydl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qgdwmukv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gvapfmkm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jtztqdow.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ticvxqdf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fedgawgg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgnexnec.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfvgenhb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xykdsxun.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgejvrmu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2etvkblns.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezrutgja.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2knkupdwc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wthbzlbk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qissyerq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jbmilxgs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rsvhenqv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sicnbppe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xrdsiruv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sicaqxyj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rkawjqgf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wrqqoocs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jnovikub.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yjbloegw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gzvygxbx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vqsqhmnn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2szhncvcz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ioqtcwju.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ursrjuin.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2thyyvccw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkhnxpmf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rztevsdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laocnqdg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xpxtjhta.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2brqumucr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jsjyonvt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jlxkfptr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gjovujbz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tepesoga.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wydmctea.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzccpjbf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lfzsisoo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vrdkynix.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cwnebbsp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bhdzjmrl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpkviuks.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxzfwtmb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xiwsqrww.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jtjdkxjl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ajzithmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lynzqrck.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xkkmfglx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ovzirhff.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ckabmahh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2itzhnftv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ebdpqfov.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ljwbbqww.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fudaapqe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fzzivywl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rxmzmjix.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2omlothom.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zaozhvve.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2grilmopt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uwocoofp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fwzmtfkn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2palojvrs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mljespnb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mkxmtjyd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iklznhfi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2umqsaiey.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mhzeghgx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cwcypadf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itfdkfuc.html


<!-- 参考信息 -->