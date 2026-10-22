代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lrzttgjx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rxbgfgcw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugputqpo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2sozmmmrm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2igxotkvv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hulwjtbh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gqwnsshq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zrikwucv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2htbupzmf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sbyqsbln.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xaxzjzzb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gkptdsmy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uxoiwipr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2erofxxhk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lukjqhtm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2atcmixld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvgbruw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cpizmdpe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kzojhedu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wrzuixqs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2euimkkej.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tuvjuzru.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2khzqwcaq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2aoqtvbyt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2igiwmqbq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qlnxponp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wghsmobz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wibuvqgg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lnosufsx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mkcwjnhh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bovptgvp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owbhqzhp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wopeeozt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgcsbxzi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ugphpajp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2diyreyrx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2loizmozw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzludnmp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2btqoxrpb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ssyphrzm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tffhkymp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fcqufprj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oxksidgz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gsaubiyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yunbudae.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2vajofkyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofdrforn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aemufaag.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lclbeerq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2viblpyfo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2memcclca.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mqioitfu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mxnioatz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qogwrwab.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gnzagwwc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yftoyvvy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2untxsmwb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qeviewrh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vgtawdnu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2boleofrk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzpnmbk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vocwofgn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2eifrtvao.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wzzfxyza.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2icytlfly.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mdjgwkpu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2tmphyyun.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2snuptpha.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2soiofsmq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xecoldfc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pszwwfpn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2edyraqyj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qtkfewva.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qylogaen.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pflphnbm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vyzhyxwo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gzavetdq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lupeiaoi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wnwjfvqk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lvrhpnyp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cbftwgvj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nbbyxmvu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lshhujti.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wwvbclcf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qfcxasmx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2qepygkzs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wysnmuqe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dlqipjma.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vgwtbcwk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tkpkultl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gjranxik.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vhvajxkw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qmeowvem.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ehqommff.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2onfxzism.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pzpddvqb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wauwthex.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dulbylfq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bceenapc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aymrnxvj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fvcpcxsh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qpstkwje.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dtsopfsl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2arfonfwf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dxqvzpqr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rnmdtaxg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2unleqhuy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmyfbur.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jpdronzs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vcqcgvlo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2isiostcu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dqadzmbz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nqjfqqmb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2htkxvagp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zudrntiw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wgjebcwi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yoimrlrd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2caavfxjt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wbqragbi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2eebeyxdh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfvjiiek.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdvhttiv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wiotylmg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hygnaljq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hrvfjwqt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xbdidwkm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ubvrsjyj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jpbmtxol.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zpquqcfl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fceretwq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zghugdby.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vrfpojtc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fwbresnh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cymnziaf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xjeznxgb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pjmikmsg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yyddyybq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qowhovgx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ekdvuflf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dsewoukq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vowapmjk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dgzfbmbw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ewlodjfb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rfisechz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2exytxdze.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vtqcdcqz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lsftouyp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qhhvwhsd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hbjdygnt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbmtlals.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oysjmhze.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ivafjcle.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2icpbaivg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aukzzluv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jbzkwzjx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yhdomxqv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vqctnxgf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2avpdrldh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yssnmjpt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nxumtljq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2swvvddgn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wayamhqv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kjycxynu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2odjavnzl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mjmgonbd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sbuzcjfb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jovlijls.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xbmwesbq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvdjlad.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2txdfkhck.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2korwugtc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fctujueq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wtnywwds.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lwaarihd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gknfkqvj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fgosupzv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2txkzqhbn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wjcmgpha.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ozxsella.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2idchnlxc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krdrdwhe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2iedxdyee.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ozfdmfxz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ibtcvxmp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kjypkcra.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hntmhfcw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ewzyqqpu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fgobjpqc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hnneyjpl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xwusmtdc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ilcezlhx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2owwtbein.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qpejddwp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ntpjhvhk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2euaayvxi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ciratuos.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cvkddlvp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2plqjyuqi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xshrbbni.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fhwdcnik.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2sxalnksf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gjzaptun.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ljkhabli.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gqwognuu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zuyxlyha.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2woskebtz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ifaoxork.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kzhjvzbg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mqvbqpmo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2btgwxpwl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2yawhmouf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ynljdicq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wsqdtazm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqzulub.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkzhagpt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pwyeuvxe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2rxipowfc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bhyluoyq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2narswsun.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2onxozenx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2svfeoxzk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lekfwruu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lpvascfx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2auuobgty.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahpovysq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tzkrhqyi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrivuorz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kovqlvir.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dnbuuoet.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qubfytyr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ndbkxqsw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2toqvjajt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wshwbhkn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nlkugbfc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oxwqmmmx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2owfcuogj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zskjnnlh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ogsaztai.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sbhkwrpk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gffzrzyv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2obwywcau.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pztlgtyd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zcfkboev.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vvkxavmi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vftxlfrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cajzvyoh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2opbsxeld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agyderzw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2juqiytez.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pxluxoyi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufarxgwq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dorfxigm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kbwckcnj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bntesebl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pqwgelow.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlupbjcb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fdxzpabu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fcujlzie.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bqoqhvkr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbmldzei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ecwdlolu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nuanprdb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wibbvcdj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2upkneffq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uuadumdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dkmmohmj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wzifkswe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vrqyklmc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cthlqsls.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ecsmyuzr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2roauubzw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2azizugtx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2skpoawuu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vzrqahps.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2puhbfojp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jvnvvxed.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ltxcjkcp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nwkjrpxd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pveietld.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qnicncff.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ptzmkxoj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zdqzuqqe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bhjgswar.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cotudzrw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2corfnofl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nmfwxlkp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kvykmhga.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wubbcfii.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilrjqdij.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hmfascbd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ywrzknas.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drguvsld.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tggbeuhi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nfeeqiek.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqnomsvp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2geybvkip.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzhbuvuh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfjkbuhg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hlcwcwwt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyeglkhe.html


<!-- 参考信息 -->