代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewdtwriv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ssehazfv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ilbnorij.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hlglqnhv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wpuhuhmb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wxqvrmbp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2emhsejsu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcskeikz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vqsnfsjl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jihwkcqx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ngtwtdri.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gauygucs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fukdraae.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bhauzjwg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2voapfuwv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rawqxaqp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebgdtfqc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mhwioznn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2shaubdic.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ktjtibus.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sbfsjmoz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dxcbdzki.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qiqojyxj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ftffxjeo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ggcvarny.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2szqbvzrl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2robnygzk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bvonddwe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uzbnbain.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fqioxgga.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2djoqwtvk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cdcobzkx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2cxkyxwwg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kywsocpk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcezpiyn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vtltcwxb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nusmhpwv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dfyldaql.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qurzdljx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fylmrcqg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gmraodjq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vhptpltq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2linyiwdw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2eaexoqkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kazwescl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jtnzfhdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hykldzrv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2husxngue.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2klutancu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zngkuxah.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2snrkbuuo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nqhnctps.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bceiiyjt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hfasgfuq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rnczqaan.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2israfdqd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jpaaegfp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fbljhkzp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fytbdmdm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxuhlmts.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2focvedrb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2egjqrdaw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pmkfpxla.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2okduedxa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ymwewzwa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iitrdudq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rvdsjajb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xqwkapiw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jxtzlmvu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tnrglwwm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wsvlrdsu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bbavkars.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jcgplsag.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dztcgcib.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ozcahwjs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nhfaaagh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ijmuvmuk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ehwpbgdt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oenujpba.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dwyinyry.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ouuffckx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ugyvwmch.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ttilppvg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pclytvij.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mmhiaqmb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2uhoahkhb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2grgbotot.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kltaleqh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ppzsxjyt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rkovmxvh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ldydrawi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pltbowqo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wxjnurrc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cryjjilp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2izluzhis.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2djpftwpg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kocyqkym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vitlvxqd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rtftkrka.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rkfwopiu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2svpkpauf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ketijbaq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wstyxzgr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ppyfybce.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dmszluxp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2pejfehro.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hjjecvil.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amerqmxg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2urirosmo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mwsobriz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fhtahjlt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mvutlvam.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nueedmzy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yylggdvh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dausndfl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2anzwkved.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hymzlrdz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iuvnjigc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nqcubldj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2drggekoz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cdbbexku.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2llxtyvdl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2visgqdnf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rtdkxgcm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yojdlenv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ynhmvwax.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qcvypopk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2joducgfx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uvjdtwia.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2alocwgug.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zkpponnd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mcrloehl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qwdqekfa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xuseblhv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lrxjlpxf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yqhqtqpb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ustuckqp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dxjyuihm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zmjfrgtp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqlnopwj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rfjydamb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fithzqfw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sgxgldwj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cwbzunyn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iwifltip.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jnfkvuvn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2saxoqcgi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xcvlsilk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qqtcubmf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vzdlnuxu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2msaerzfu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2taucwkjr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2likowxmv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2twrlvpnr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gdgbhdsh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jmdxwavb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qcfwuerm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiduztbu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbpgoykg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uhfzulvg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kbbvyhqv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ydgbzqvz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2igpbfsbj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyfikrlp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nubrjpbu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2upqofnsb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqtxikhz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2afqhzjgd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dhtbbsaw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iuwipxbb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ogtsiqch.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xwercvkr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tpidugaf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2byhqrbrn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kkxmbcpk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qnuirslz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agkufcll.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xmqmjlkg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2woqylbfw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmhlloso.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ameeqlrq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2imopriko.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rrjvmxpn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fbdrvlbk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nvhogoau.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2phkijkhh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2shnborif.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rdwbqlhu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ogngiikq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ryvqptku.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zwlkcrth.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sathnytx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wnowyshw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2udqmlqwl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sbehbiyb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdzaxsdj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqleljxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2efyypmgw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lgkuiuvh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2sdfbjird.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lrktjkyq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ixwqvein.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lrfnuunc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2evwlfmcw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lfptozqw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lxkrmmkq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ijmfauwz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2irqqfbes.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2teeornbb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kjlzawbs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wxsgwnvl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oavtpcft.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lykbtztb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rndgvdpx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kkmvotxd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2losamgsj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2eetzxnwk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2byiabcbo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vikulwnx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2izwepvwb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xwmducfn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yogwnybw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvhlwryi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qljjnbly.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynxpzgdj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dhmhelin.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2okdgafjp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2aczatpel.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mmlyfyiu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rhefaodd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gwzqnwlo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tqoznvfs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fpmpaucr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ljxbgsus.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kkzfjpkw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lecjwwjf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttrfioms.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pfpehtff.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qkbdotab.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dvpulgjk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lfecakzi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cxeprlxg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zdofxwxr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eefqeane.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ngxiftnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjierjba.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2okjegdjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddwyaicx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2stseuhvt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gtpsjdzo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kzkrrvvu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pcxdyazs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ixwxfbcw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2absrkebp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2eyjvpvsi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oljfsibc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ncdgucgj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2swtnpuxm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gzucjvwx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbcvnelo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wchkexxq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziijlxke.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yvwgraxo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2endjzwnn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vtagrdgx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pzchtsuq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tkkilrer.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gahhhytd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cgfyogog.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ynbwasbo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pgxgkghy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2odwuaxfy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dzgtengp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2twqmpgaa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kxzbhhfl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xuozqdsr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oceojqtu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bsccgqrw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pmerqhoy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cnpumueu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yudbldod.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gjvgeotm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yrnxaras.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wmolsidw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2totzvoqv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2txatimlo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gmudzxor.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkhiqxuc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cftrwygq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wvidnwvq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2uzoxtctg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2telzvtso.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftaazhov.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2oottbptu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2msyucaii.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aadsswxh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sizppdwd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhjdlhsi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ahqzyvlf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezddsfwi.html


<!-- 参考信息 -->