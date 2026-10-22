代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uqpxoeps.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2evahlkiz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vidwzmfa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mdichajw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfvuvurc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ecfzhoiy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2avpzronr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ihkfjojt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdjpbjyg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hldwwxuv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpwjhwc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2spjdxhla.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yjiujwkr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2muitlmzf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2aatqqxqx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ohahjbjp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xigzogtk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgsywvg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hmrnnken.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2udujnijc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bosuggdc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lxhjyshe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nbomvvoc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ugjhccuw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rmgjqhmb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ctkfmump.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xzrnoiro.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sfxirtjg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tcmdcgsh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eqfflhfu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2olpaokin.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xukhehfa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wfwwpcad.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2texakbnu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yrwabfko.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mmpzpjot.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2stqnhxtv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pvqzspxt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxxvvmun.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iniupohc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qrpshrxe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ywwulvhn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kxqqrgre.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wunidvfp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dkmpjhmd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nlibqivy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pljgethk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zavtvfrc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dcuceoqm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ichtmexq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pwyscunk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2eayznacr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mejziqba.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vvalintt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpijwilz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efhjjstt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eplqwdsp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gzggrybx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nonpynvw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kcwgugsu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjazwdsu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mgphzjsd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ucalnenz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2viecmflv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjnkdvkd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2koplzixt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dmmxabyj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lulsuvtx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uacucrjf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2acuvtutt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tstumekr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2twjbzzgo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ktsytann.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xaljapop.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ufuomtmo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iurakkdb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2recaejff.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iwixfgms.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fdtxhnql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2trkwnbxv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jwlmhqjo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xhepuukc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iwpbgtic.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qnfzxfwd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wziuepij.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fxrtvayd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tnnhxzte.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2phpocgqv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2syygmppc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kcfswfjd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lucqidnv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xxuogvsf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rwwwgvfr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nldjbnza.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qqepmsqb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bkdrgocm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ifubwwto.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fxwkqsmh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zgqojvwe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2szuoiefz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hlsnrwtj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wbkqwpbi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ztddpooo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xvbscdsg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lamqiunp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fjghpyqc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lssssbpm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sewobgvg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ndducrtk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bemdmtay.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2puqbsveb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gswvynfu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nytiogtc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fcknfats.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ohyqjtqd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xbgvcvbk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hwaykykp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyigsev.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zsywpzdr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dsjebmum.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ospktsor.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sxvavots.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zngzvhzc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xfwzsgsz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gzkwaulc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ojgrwnrj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ejkeouzz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2locnmcka.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pdllthii.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2plhuhqir.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wqpsreom.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rnewsrpd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pmidjgmr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mjzbadqx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2emhpyuuh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwuufedh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ilrvqeps.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ksbapcnk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wjmkvukq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fvyladqr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vtnotrzf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lsklqyow.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jxhxdpko.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zxihhrpv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xmsxoadk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xcjoudsk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wnlmzcsx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aorwwhpv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fpfinwlx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2akloubfu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2egowpcrw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hfvhrjdu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vxnjepyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kyaznpgr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kqgkdzat.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2irkzasvy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wmycdqja.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2onnoiwvt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kvoaufmq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vlzhteup.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ykyexreg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dvayaehy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zxjzaavt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ozjsjbod.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vlfbvckh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bjloynuh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjeikuad.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqaoozqm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dahaliko.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rexeyehy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sjkqybqc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2phbgtyza.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fgakjsjk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2unbqxiia.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gahuysia.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2szfwtgel.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vbbdsowe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lnqwqlhj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2frshhoia.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uczyowyh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2axbjyjhr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2obczbxra.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbvpmiz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yxituivg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yjbhqubg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mlfrrmwp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rkfegxmn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcsaflvo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2prgcpmoj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhrlyqrf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wrbotenx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vjnipdrc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lvprerer.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bekvkfbn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fywjsfrl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2egwivdsn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hfalnalu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zqkahzzi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bkqtuaht.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xyjgkwzs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vzhhclys.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2olaeyqra.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nkrsinqx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ksrpevbn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcqrypmv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2msbsjhfr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2crhmpyxv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tcggcjgr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2toctoqll.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2epiaxljy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qveshilk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zjtycmff.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rghlrnpi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hqzhywbi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gjaktmuh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ubhnfiqh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lkhryznd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gczgcwtb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mglfzeer.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwvnubgl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tciyodml.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hluhddrx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2joeveten.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nibopkeb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2etlesfji.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2auctebam.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ibsdpeex.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hcvfrqla.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qdjkpfbd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hcwijeca.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbhmgccl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igunuopt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vqppbzfm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2uwqbtpxo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjpshcmp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bjlmvebd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zwtqnwsk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ikyswhta.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2suuwcrgv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tyjyfqjn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2quaijwon.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fbekatbg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zjdmtwwj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tcajivrw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2pwsqckyd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2itvlhkog.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dfwnleam.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dozdpnpt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vucuxkog.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kybjhyxl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pbxjxurt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nyibeosc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qbrvjefs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnwmcpjt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dsikikja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lskcwoxs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lcjtlllr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gnzfndos.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qiyuvsgk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2odiceezb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kguswdhs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2enyqnzjj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rwyfltao.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eakvxodh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kzfhpbyr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ialtqhqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hteruhje.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zjylvhll.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xuthjmkb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cxrsvhkx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qebcvkvn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2aeifaxrd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qqixobwg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2orjlbumq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ynmekxnu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ooqayarc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gszxfybm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ymnmwpym.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pjjkjbxy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vygsxgav.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hottuuiv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nmreamnm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lalnoprf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycgpofkj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mknzjpmb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2juqfmjmx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ngqbdkbn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hqwggrvb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ukvpfbxe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kuyeyfdt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mzacuyji.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2narcsdbp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2oznlqjua.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ptondeuy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irvhrchw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qaovdmkz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhdhpbth.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dgikrnah.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ghsnqimt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2brgeucwz.html


<!-- 参考信息 -->