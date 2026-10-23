代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ueislxet.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wlixsnva.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqocejiw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zsdisjjg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3epnloyuk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zczinwer.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3thehmxjb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vyuarmke.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oxwgprtg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3znhebqgj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pualchsv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bqldmsjk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tofhpkhg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jfsratjf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3raxsqvle.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3soaoirqb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xlaloivw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pyeiaeif.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wlmhcmpv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ccdxbfmj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3iphjadhf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vrwpwykk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ywbdaelx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3awbpesrk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3guhbrmzx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yvtsxqks.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3proqwtyv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ypcjtoyg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3slngvros.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hypdpodn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mukvwhia.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cswjctcg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vjuvkwzd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqjvbjk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dnzewoof.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3oergsina.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jpdjjlnq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zedzwmrg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3scpejfrp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ygtfmxym.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxegaqo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rftaivrm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mnnbtqxa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lkhqplpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rboqfgmb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bkzutali.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwqfhpgs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tufhdire.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vwcupmhh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qaudowse.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qrhfcmht.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ufblhnlh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3muzndyka.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dfgwsmld.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ntiujzal.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3niradonm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wpatcpwf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ykkpgzbq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3obnochre.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iefzdbaz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vajxoyov.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fioqyeij.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kieimtxb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tjwmtphh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3juymznhr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vjzwucft.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hyntusha.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ftggpfcw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tleqlmds.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ndbutgkc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ikqmahbp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3phgjunpm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3glgjkjlw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fbdwmpvz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3uqssxcya.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tdcwvomm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pxqpwgty.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vjiyeniv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bwunomli.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3osetwktm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ziidwqfd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nraiixts.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3olfjyjxp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kqcyvhwa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iojsrsto.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dzpapwzb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nbmqxxzs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kdyuwfyh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bmdqyhyf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bbjxizhk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3meatbvtz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rakvqxuh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zszrpigx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xdedfdeo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sluwjhwy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mwospyur.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jxdimbfb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ddxoocbr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfwwezh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qyoxtxvh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pnnkzgil.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xxpbvwox.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3oyahwhva.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxjpmfiy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xniclyex.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tbowjaqf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3afdztwut.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3uhzleyei.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nvyqjpin.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcplsag.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hkrwnfzb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3uoszvesn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3olvuxfnu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zxbqjotd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3khghqayc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oyocbkpd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hfcbxkod.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3olirhngu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ysujrucr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3eyxccpir.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dbljbjxq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3mqdazkaf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qlsvxbdi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jfvdfyyt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kxbbzfsn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kuzbrzpz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pphflhiv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3elexqpkr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wbuhbxju.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kxauthuq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ygzzblqn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lxritqlq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lroqqsbg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ggkephvu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtqkzvl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ssprvror.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3yahgmvbx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qfvmxdqy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ddzfjrhu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qbrsrmsu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oambdkvr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bamupzdp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xtrmefzk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mtcyqgzd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3phazptmv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gurbguwp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ypcztbno.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3umvglfhm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3udxjhbxw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hpbwhgfq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzowjuyh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xxeipcze.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3onqwdhby.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ekijlvgh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hlwpwpup.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rxdwgjgq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jzqxlcke.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hixrclct.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eznxiecs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpfuyfl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbotxpox.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ptnoioxu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bxhwsova.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ezhyzedv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ahespkyv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3riatdbrm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3abojvrpu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dpliaduf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ikuckklj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eshthgqh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dtxmbvxz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fwzngrmj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cowunese.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bvxoyqal.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mejquolm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vojfatuz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wdozalef.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dywazqmi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hsspkjhf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxuoaxd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dugpxrbv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pystdjdt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ebzyhsxp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yhqgpesu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3oddxybme.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3anlojkxm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nhoflwku.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jmdfflus.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3assxwrye.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uryjlsia.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wzddubme.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rpbaygbl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ireptifw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uuutyntb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lwckugwu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3crqizgkt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbbugypv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3keeftnxh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wnmcerhf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zapseljg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jvfkneqx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3eycefzcg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kdodwqvt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xtvfeysu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vksjkugl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3flyyyqnt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3liztiduj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3orsiyltt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3usoawhrr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gzumaqlx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fxxjieat.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhzclttl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zcefqbar.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lnfwrqon.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxuqhdsh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rzrdiygs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3uknwadrd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3irrgdsft.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3slnuelhn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zvzjprer.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3efdhrlls.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ngrbhqyo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ologkrlc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iydqiqfi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ltvdnneq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fkzbpquf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swrbornu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xakxvjce.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3srnwiwba.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fkxfmcqc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3txvvjisy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oiozvcyi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tuphyvjx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zumchakr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcvllddo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vzuctoih.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ercyduyd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ooeptbql.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eqywvzbq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qbasrkgg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qnlatxca.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tmolszkz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bebbmcvs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fpymblcw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iktqpdyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abpgzkcr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hyerxcmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iigrpcph.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lljdwaep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ahqqodna.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kcfkvogh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jpxkibie.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wzqyiivq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3exvarjdz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dxsjzfob.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qyftpayz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxizbgxx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pwxrbjqd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mvfyfnal.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nsaylqjl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rpgtfvtf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfcgipzy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhuubza.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3iugtcgrz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jalebwbd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lhnpggid.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vgglxiyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nntdfhyl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nnbnbqbh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iqhxtvyh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3croahdap.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cyleixbp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kamxjnqz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wtgcrsvj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rgzkaswm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvrkkpot.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rfqfanwe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ylznrrsp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cszsnltv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zpxkmlxe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxulltl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3narwtddu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ogrzkxqt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3feabqqey.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lhyzqxam.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vcdakjbv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vuxqdtyh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhkefagj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bntbtbae.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ipjrghit.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pmhqdtxn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbdccedx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvnmzqph.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztbutzvy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkbpzcpj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tbufcxfb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikdrfgbg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irgoagfa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ttcauxpj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkgssuie.html


<!-- 参考信息 -->