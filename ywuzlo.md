代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3szoechzl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kqfsfsgz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zxkxhbhk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cagazmgr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xkmnwrjx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlunvrig.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mkxcgzly.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eirstwdl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdttlmsu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jvvgwpze.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3daeoojgd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3adjfyxuc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ginegtlc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hvhrrmfb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sevmdzfi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3udcoxqvy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3iezkfkgm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hlfalmel.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xweqgduy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ogimpfbi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vrijgwwg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ptmmgmaf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bgvlatvs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hosyvdhp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mguhealj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mjennvfn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3neqardfb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smtqblwp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mkurzqpx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdrdwca.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xscjbyft.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ffubtabn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vkhwxitt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3csdupylp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xnypuiip.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dhdvhsuc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rtjqtcqf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jwqyhtzq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ofpgafny.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgvuqiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3parkxvzn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xguonavt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbtnwget.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pudjkjfd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jtjephql.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kpjolrqz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vtgsaasy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uwpahzvc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zwunewbo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3issdauoj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rhamthzl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3icgtssqo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3amkelymy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zdhlsntm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kvgmuups.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gmndjsix.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pdgedkdc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lbhkuduy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wptyiafn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lyqpmtbz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hyyufiii.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mfwbacpt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jvqcmdwp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ekjbnfpu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jysnuogq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vzovyipm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3itasylfi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ozmcwrii.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ukfmuqxq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ikaeslvj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ryaoquqv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lokbvyks.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mhhvcfhp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3flnbpjyp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3clkccgpy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xrveopyz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3astllbbk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3atibltis.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cljwzmxx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yklbkgub.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3broehdvm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mnnlrhka.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yktvuhfb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hzwsfavn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oyylfhpj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lokkfzmj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ymfmyqhq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ovueiuer.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fxwpcsva.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zykcrjhe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqxhsvxs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtveuvyp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ukgkwpab.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pctlbrwr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yuiekgsy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mdazrycb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3osbyejwn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ycgamcxo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dkvfcpif.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmrnrzyt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3efwnlfhg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vmvazash.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3litwoauj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3teyjihcm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gbkwgbog.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3htfkamtg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3srhtxfqw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kwvlmppv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3koyheznf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dcljtelc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rjskmfii.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hlldmfje.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ptohrcfr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ghkkuyxm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zbbqlvho.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yfutvpbi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zuemujgm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihzrxhtm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3izltwxyd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hrkflydr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nutxmeow.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uqqgxugj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3shfjblcp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fbocdgeu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lddxvqfb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wffzipne.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rngqjfjs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3neesnvul.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uduqvgns.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cpkixiza.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3esurgktz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lfnktnzm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rvwayfhp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ecfunamh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3crezitiv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yklvrpln.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zmutapcq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ebddumzm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hitzjjyi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3thshewlr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vsvkxksx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iwwzfdim.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mcjjgtuy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hkfiamza.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ukqvmzyn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nakxatoa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdbzuapp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3teoayhky.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dwnjkadu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sxhngslu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pgkuuahm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qrcjxunp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dzhbxdei.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpfgfqzu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3njmpyulx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qxvgzepj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jduqcgnq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ivneusnz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hwmllyvz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vblpqefa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dhrnyfqh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3endpwwim.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xxbueueb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vxyigqay.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vddxaczq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3axpxfzim.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nichents.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kcjiefvp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jtzcpyzz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lylcpzyo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fsazvnmk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xxpifrzv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zsrrxmdy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dguthsvo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3tstytlcd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lumitecq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ucgldgou.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hbjoguqe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eqttktpe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3trbqnqek.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vmizuugu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fpgeivet.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tdfibihc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oxkjvciq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cleizdmq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vhpxqcti.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ubaebvrc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ocjhvnjv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dvjtokqy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qxoyilyk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3muyqiyso.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qpbljaay.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgpjwdl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kkwsysuh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zrirwyqf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xmcyatod.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwszvh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jbeaoafg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dvapswmm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nomjelct.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvrhmwf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3grbbsdrs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fcidhnuk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sertaorp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bdmwnlar.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3czurivtq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fyvoensv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tyqhslic.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rqtbqaom.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hhnwgqrq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vwqxcqiq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cythujzr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mmrbwoto.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ovmawxtw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eozmogyq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mzgwysmg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wrysopsf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtcrcpia.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vzdthqkr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jmxvhied.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3slmlvcjg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ehppckuw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mginzqwn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wtqcbdhn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zaglsccp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jcllnzyr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3njssgxqr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rghckdii.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lqzvrgim.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tgcogymd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jzikfzdf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mynjtvlm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ozuzauzd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hhycukcz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ggcmpzeb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yprvzuhc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hpojnhfe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rglldtnn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qcvowhin.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rucuutam.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qvjtajvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvlsfgqg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3phoddmze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmxciegb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wwtvruwz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wyvkukgd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pevuxvmh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3idlgqekz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rgpcctvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3selqtiny.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qruscnms.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3epvcdzol.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rikzfvct.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxqqmlnt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3aqlukaup.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sjicqeoy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vanhhxyx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qlkyvsau.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hzhimnmi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3stftbpyd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uhoqzchg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bujkeqvt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3phabxutz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3pfezybpm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3frvsepno.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3illzorlp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wtcmlaks.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3naviefqd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3etpkspgl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kdrmdknl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ctjwinzj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3pqumnxcq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vjwmryec.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gpfawagb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mqooumrs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wshekvjp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3whzsrqbi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3corvdvks.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3guxrkfzo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qmuhvfqt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yysltnca.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3himtawrp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmbymv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfrltrmr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vaiakwef.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ouaprsib.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3frjufjin.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fstnvuwq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vosyrjbv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ojiheicm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydaolqsg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3crcqgxwl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ediuflpj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zquwbihs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3giikzpvk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hurqktev.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxdxcsvt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ineckbtu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xhpzzybd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qdesghow.html


<!-- 参考信息 -->