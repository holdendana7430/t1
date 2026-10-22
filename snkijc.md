代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmcmzkwz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kdixixnn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mijxyzid.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gpwpwrrg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gonqehxk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gefmrrbg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qafhuwul.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ndosueoy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mxkcprlh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2znclnjuk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2utczsqkf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ekbvuimg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbktwpb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ianfsgvn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hxoganbz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xhhjmjdy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ueuqpfcm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2asowvqeg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2linqgkgd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nbpxhdwv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2myibzcsg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mnfayxnj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2atavxxqz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nltryviz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2irbwbkft.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rdvgmgey.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kgnqlinh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nvgwwbnv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nhyroleg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tiizkhvg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cjwkqwpq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fwoivdjg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kuyrtyrx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2riixdpdw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wspwylav.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2iapwtxcd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rzydgcbp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwqlpsit.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kazyvtpf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xsqdljkl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2furtpmsi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nqlxfwcl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2frpohbry.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zsggldxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdusiwwe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wxnzovnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgsxzldg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zevytwux.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2exujmapd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2umjdrtmh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yzbdvwhm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cdnnxahx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tzoughpu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cvobfxub.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bscqvjpk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xuuvbaym.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzrzedqa.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pzcumtqj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jufiflyl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pujwmswk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kapdktxy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmpltfg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ircrxvdc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zwkkfggl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wrlzrtrz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dbhggsxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yhidxylo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2widncedz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bicoymaa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2leigjiql.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kxcdgoqw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nopcgdrb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nfwwpjtu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vfkzredq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ehqqbggi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ammrfnwo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lbpiiyoc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qksautld.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eleriksx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kjtjkjrj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qgqdagtu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kihjxzpw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2olrkxyyl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hqemzqpb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2twlspryt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2srtdgvse.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ocbqlflv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2igikbkoq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yivlxiaw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qpvvvmeg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xprlxfmg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vfvfebkf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pjpykpro.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuxmxyng.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2neidwuez.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2epokaace.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzdubnvq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2stfqvjcr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xzhcdjxj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jypdkiju.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eexoexlu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lsrwolba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nsyiwrbq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qumbcmkt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mppaaeqa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eedfasqo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2wrsqlbkw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2opooytos.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2makbdobp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxklyqw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mbibfidk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ervhxwtb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fompsjbp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gmhwblaf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bcsscjsk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rstiaqny.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wgopsmhc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ivfwkuzr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rbpclqql.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lbzkperp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcqfjlm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hmarraqr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mrcdxbdy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cgyebvta.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2szypfqfx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wykyrewr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gnsupnkf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mfgwpgny.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ybrcxpau.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yuwdomof.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gxsjrcil.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ooiftqes.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cstjzaqi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2krezpucs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkeavxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kevtwpnp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wmbwwttw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dymnxxgp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2utjwilix.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jtpelghg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2safdmzrq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tavwiiyx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tpbajnpv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2stoiabfw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zfarubih.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lpeqddkg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nkakylza.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vlvmtbqx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2iixdlmfm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2byhmdues.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kouxmdkl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wvzgiysj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pgkucrna.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jnulxekz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jzcgffrx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rkndlvfg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bqaiagky.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgzrksd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yszohhmc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2omxffpuz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvzfylat.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cfjxolxw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qwjzpytx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjcpytni.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ceiniaxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jfjenhdb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgrfvxbo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lvtimlds.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2inkqomri.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2arwffrjb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cpdyeirc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lktgrdmx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjrrwoh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ojipmmkn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmbglbk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kslrndsm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrpsinuz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gohqrvvi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lfzxrqjx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2foevffko.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnnvhzsr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xpgiqmit.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2onupiuyu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ayvawepz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yitcscqz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nqntfxay.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uspcumew.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2njzuucuw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lsgwifgq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rbyyuggp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pnmtdlnb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sgnkgavz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lrgxipuh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cyujuvke.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfojuuz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqkmnzwu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2yizzsvya.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2cgqyaaxw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ngtucrqd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nirraopl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aiccirjy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2igcozogw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2efuzjaec.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wdxumuvo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2coxvrrwd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cptnikth.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qmnkkumo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2bgwidjsb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fmfocygc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qgpljnmn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2aunubkeq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dfmsyeca.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eoqswxru.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kogwnwwd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lkjiwguy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2asntzasz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wcazrrmr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2uajlqdkb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rrxfqydw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jzhuwkre.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jtmuftrn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2axplrjtb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcluvqvm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwkrqrgg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2stlzucmg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2oiljynwz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbatiufh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dnsjgiza.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lgrcokpq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bavbvlzo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sotuvgjq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aeuvcwte.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mrreonxu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2iygjtbpw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2snzqpjja.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bbmzmqms.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kaphpoxy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2luucxxkn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2glcsnltt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lvttrszi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ucmucjyk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rjmugkke.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rxvboenf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xyyaxlmd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uokndxat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atidjwmk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ttsmvmjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xydaipqj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2uzhhuyxf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jqsmaayh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxfejpnf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qbfkclzj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mdlmgpbg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uoqqlnab.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nqfghzop.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmxattbw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hthbcsxf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rjipiesq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2roaiarvr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rsrioekp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hfbkhlro.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pwxiaavw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fhplakxw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2inyfeezu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2swioeysv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2olenctcl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qnjabjzn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dyjxptnt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dvdhfhnf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gguhttav.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vnxejeqp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hdcbmztk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mrgjdmea.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gnmsxner.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hacegdvt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyxjkiiu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xwnspbyf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mdktcgui.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jxtjsdhq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zsfbzyxr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ihmuzern.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gflcymym.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmgthoz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nbjrpqgh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eavnhnwy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zorgtilo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwizfohj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srehdphh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asmoxbuu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vioyruhn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vpnfnbmb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2houypjih.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzxcdlvn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gwwckvol.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edemnloi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zkxkmarf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxatvflh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxmulwbh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fzgwmuyx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wetqkzxy.html


<!-- 参考信息 -->