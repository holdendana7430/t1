代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2igmtobte.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wwyowuqs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kimldewa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bkxbruif.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ibwpfkqf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2emqylcfw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zlixxjbw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zzjqmvmv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2knkgshzp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tqfruyqr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uvjkyfga.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ekubtpwo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kekamnll.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2phzpfydn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hehvhiol.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bqskrsul.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvrmrygm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ctnjomgu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qfippxup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bgwqkaxo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ocjanreq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hdycquui.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qrunyqds.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wksqewfk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pytrhofu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edvjorcb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2skhzodtj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lbokqzxy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qehgyktk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qysrerjj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2urdrcgxp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzppjhfy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zubufurt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqgrgbmz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ruspiysj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tnmmjwac.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2waoiibae.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zubrilpp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zrlcjnny.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lyybdigt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyvdeuaj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qrdraedl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oawdoctp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2evqwykxx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2btqxwnpm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ltncwxuh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bubnowvv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ffryvooj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbyjrdrn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zbfrmpsx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mvdphxoj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xdhxuihw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmpdtvxc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rogspjnf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zhwrfxln.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzgfwxkz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gttjlrbq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxcafgw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lflpaera.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bbqbhcfo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cyxsywzm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qncdwuxj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rprshlda.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nugkkyiw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2keoiybyw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dvcsgoft.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hmvbaqkf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ggexfyzh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tujsnqjk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmrjzuml.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2negtccyv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yzdaczgg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hzmwrlml.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lenchchc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fjygxzav.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hjbbxaqu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jlwgaacm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2luispfbg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kppxchwi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gjhgenwk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fnxeqnrq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ncxdoohn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2utqiqhly.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2onernwsv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dfegcthg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2afyeduef.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2orzggtaa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xhgenmhr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sxhttimi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dmqezfox.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxggspzs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yxrisfpl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vmhaukjf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2udclvdij.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2khwodydu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wfffzfal.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2atasaacc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pdjscnke.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ikexixlu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iyxixgmc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lqwjicbr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2scpnvwdi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zduacmrl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xxdxnddb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ubsodlkg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nmldmipy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bpfjznns.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wndksbji.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vlcxzekl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lnvtctyy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2budkjliv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bltubwec.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fmbpmdiw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ucyqfouu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2spedvvlz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2uimnaned.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2toqroswo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qppbuxzy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2enjznlox.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nnkakvyw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jacpvgoi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vwyfrgqq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2afubzdgf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2paeodlke.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fvieyhqp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tcpyfzcr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2romqjtbt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2llginuzb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zbvsbowr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kwsokyjq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2owmvvgbd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ynqtmlux.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ycwelght.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hvwpgnlg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rhzibqlf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gizjxxve.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aouxqapd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mdaipxul.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2afocszgk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hgawvqmz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sldpbqrw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dgqzjjph.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2riccpmlf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kghzjssa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dvjyskrr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gslnpuoo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hiwawjiy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vvhqzikg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hbshbnwc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wxugjali.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ogiakzqk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cdnvtkxu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tlwacqpr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zthtunxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hkpmvjvo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2efmoynbl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2valhdmlk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pwebhdbq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fhfusdiw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2czvekhao.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uigabogk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yegsnynq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2idsksftd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yaheclua.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fywhamhk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gkgglhel.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zkibspgv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xdtsiqxw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2szloqbtv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gfvphsau.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rpnzinwv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2corbquay.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lehasrlt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mjqlnqvi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2friiyhcr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2djyashvn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ycxeoanx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2snezebkj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vymjhxxj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vuuprxpv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wpojtafi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2egkjmiro.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jadlchci.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pkzntozr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nfevaqfq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kgvxrrqi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ncyricgi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2auqlwlbs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zfqkmtaa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isecmlnf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rkhxoouv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lufbbsii.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2khpapwgv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cwdotolw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2komprfgz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wflhaiwj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lbdbpakl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fnblncjt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uchzpqag.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bydinuap.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yxmkstfu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vfljcuor.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kkqpxzsp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zxnlyfjd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wmkmjbiw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jqbayoeg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tmdnrohg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdcdclls.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwrkoeo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bansbcdk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ozqekiof.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nfeligbe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yvdzikze.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2mnpznjvl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2yujnrptr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ufyxxfze.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zbufvbkc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxpmvcif.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2akocplcw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfskybap.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gwmigdfi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ebnlauod.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fknbrlxc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uyuvadvw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zwtztrgz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gbcxjogc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yllcemch.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ccavuudf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2txeqjzpx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2sqbixzzm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kjbybnty.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nqbdsedt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cmmeucwg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhxfniyk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jxkljpda.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pswecjap.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2crlxofvv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2znwkmlxx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hxrpddqe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tbsrrmmc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2foebkzrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qljcxibx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nynnehpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjrhpscl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mcvzovlp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fuhhzxig.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqubnakj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bichxtgo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ghhnsigv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uwmgklqx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jipipbvn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gekepdrc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rzngoxfx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kngilhow.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vuthxqer.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vporyilr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lusmqipi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rhumhixx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sxojkizr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2twmjnvwm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rgobjlyz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dbimjzph.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sjtxsfzc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lmgnufxn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nqofsfbf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qvxhoctq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xhhzfgkm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pdajouxq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2vluwjvcx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fdzkmjkd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2catwbnbe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zbjhxbpk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mqarutts.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tufdqkqq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jlcbzdvt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dvsjipog.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lqnvutbn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ekzsnopy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gizycepm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zxtnhgcr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2svlyfklq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tlohhxal.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjtfllhg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dolyhhha.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxtimubp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pwbwofse.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qvslwmtn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgrlicvn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mllbkied.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hghhfzva.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykwavusv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2artbywzn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpawwgvu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwewzzkk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wvrsxwtc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcycldcn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpacxovi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2smvwhaae.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2iyftlird.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oojaqdmy.html


<!-- 参考信息 -->