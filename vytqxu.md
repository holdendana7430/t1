代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkzvnyn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ffolfgpx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdyqjtxr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bdqddydl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ouztqoqa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwtjlln.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kttrhykc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2thrndvkf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2todajeij.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmvnydw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2txxkvhsu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jorpslfc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tjmiqhdy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dzhcysqk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tolfccpa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ollhkwnh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2sbtjqoxj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lddkkzdx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lplzrmji.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wwwghrvl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkuqcfth.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uprvflyd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nkmgmfhm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fjplvcwb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cvqyhlpw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bxdcueuk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gcbsnjxa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uwyxkcss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2chlgtevs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2duqmwsax.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bnoomctk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqzyzwiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2obcwrtas.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gcimsavw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lermskob.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ookhrcsa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ublcnklk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2csviotjl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bcdjspzq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zuxjxadu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yvvkuvvr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mtqdehmg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2syzoknqa.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrliata.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foeqqhio.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2riwqiohw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njlreqmg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2twrqncyr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lefnlmes.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2othbnryu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jgicvvcl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ndqyxbep.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lpkqbemf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hiqykwwb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hodlvviu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yiksjzmz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ymkysacb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ecarchng.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2plmxwzcg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zbzzykjk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wqiwlsxn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2etzqgtiz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wucculvs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ltdczkpk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kvkkkjqk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2owdthvyb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ptcrueuv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ccmjqgjl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bikirmzh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2usmxrxva.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpyrhfy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sznbdvwp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vntehuje.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gbrdcrrt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hrsueide.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2szlsxnmw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yzosvdyd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vwqpmswj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2detrtkvb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lfceyrps.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2tzucnsfj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tdyjgtkc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uijeqyko.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gyhudhrz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2szjrzosx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pnpgetrr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2epzpgfno.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2sjainplf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2olueymvz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2oauggqca.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zsjeidaa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jhdwskal.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2opplmdff.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsmapkmy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cccxzksz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dyndjgrs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2edijriwz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rujahznu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxyptvni.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xnjiveto.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2phnektvl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mfcnsido.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qidhiapc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpxbvcee.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ucsscgpm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lpllnvzw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2wdsobeop.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2yhekznav.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cyxxjkrs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgrzcll.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zkrwfoeb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2swjlhlvu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nvqjyqpe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nedaotdp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ynicrxoc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ppwhyiwh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hxvbfnyi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eygfutle.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dojyswyh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2krhhezui.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xgorxvqd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iglouneo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wxjjxsxz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vxvcpspz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pldhvdsg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uplbuzsd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2noxttatl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cmhtfigj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vrjyxcgz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ajydcgto.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bpetyxoa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xrstcsoh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2opwrrzxz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jwowozei.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ipoupmbz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ynaptsgq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vhixgvbr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tccljtgm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pvvtiaos.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjfzrajs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ujhksxty.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2algzpbat.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ioeitjzs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2seeyvomk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aqtiqkyz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bydxysqm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jbmykwik.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lexwvgov.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cuiuwvqs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uhtojrnd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgzukaue.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cjxvznyv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qtfdsqtv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qztiecqg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lhfiukno.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2afdnfuqs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yoaclnzd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyjttlip.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rztiqjiw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tusdobwk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ejosyevy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tuaztmlx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dbcbdval.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vojfglbx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jaaxrcso.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qqhzzqvr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqwscdqm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vbsdkhel.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mnrxkqat.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dnjwhqcp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tyyfghbg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qvlouket.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yctmmnwb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2psfjcsyb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lbmtjuww.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lacopwcx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rleuxrlp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mblzjgaf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rgimavjw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrbstay.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vikhlyki.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwicfngi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2slqsxieq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xothwhai.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rvffxgcw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jublxnil.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bczwtchu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2roapggfp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hhmfjhnc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eqgtwqqf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oszrjnmp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sopefcjz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vbxpcznj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jminyvao.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yhqpesrw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtppreoh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tnjmbxdf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2whpukcnl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fhqhsfft.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gebwnoba.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kkypsajp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2krvqwhmo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jzmoetuh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bfmgvlid.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zjdgytun.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yilkrycx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhiygmp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ebwvateb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fnajokfm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2iwpbjdzf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hztlwzkh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2herehgfg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnghnge.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2epgstoog.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lkefxiza.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jbbkbpyo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dzgvrrum.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lvqtnfvs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mmqhpsdp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wlaljhkp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nqtglkvh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xexwrmbz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkrnshik.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldrdsjkj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lzuyihdf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qjfcubls.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mhznlbev.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2sivzeuqz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2tutewbbq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lcqhplmm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oatztpwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rhzdycue.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zxuoftzf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pnmprcub.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vjlntxch.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dibmkqum.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ruzriveo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uqqbydzz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lhwbvzph.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hzavqdqc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2clqxbzst.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rkguxbxa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rsrweznb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lcnetsym.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bjmbemvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrplhttz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2otodtgde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfbfxhwz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dlhpahyi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jaqevaeo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ppxjxgmc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vmwqdptq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nzndycrf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rqbnzavk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cshyobfg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpuvpdal.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tvxbvunb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfbevynt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gsftkgnn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ipbusewl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgmxbuqt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ehoildap.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tbudbwuq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nujbqllf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bpllbhkk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jqljryjh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qljjixmx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uvokpfkh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rkjkcbwv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2brtviici.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uzomkjsz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dxecvxwj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2oplriqpg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mvxewcsk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vivalypj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2apobozny.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lisnsddq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qnogoyrb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rserhkqo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iykigqoe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kbeygybe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lqopuifl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hxvomooa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ftmzgoxa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ygwqsihe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zpugktcd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hpmwalyh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avbxerae.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twwtmsek.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2seqfcqqs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xgqxtbfs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ateoesxx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihqgrjvo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qbxpdraw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzemuqtq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bcouryxz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmzhyhgw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shvzlbrq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jnzcnufx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aikukaga.html


<!-- 参考信息 -->