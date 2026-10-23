代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tapefsmm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mmiylndy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3urwrwhde.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3chfzmrfg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fsntlxkz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tnrwnsrm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fzfdxhrk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3czxxcfsa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtydclus.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aocnkokc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3flrupaty.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fmxwvpwk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ykqyuffm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rlnmrjow.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jylxxlcm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3acwembtl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eigpqoye.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eemsyqwn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvlbnopx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvgjjkt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pomlmmkn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdwzghl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uahitrqv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lusjagej.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3uwivnubg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhmwuewy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dibyyoai.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gnnccoqa.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sdipsxql.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3iwwwfcrz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mumbwmtz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xlyijpbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acaszwva.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dnwknwru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubrzhtdj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vgnvnlau.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pzwckptw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vnarqfzq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3urulgfdw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bkblpujb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tnfbmfie.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mibkwyuf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ttulntqw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eyjsitcr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qpirggjv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jzjmswny.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xyhvjawr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3axmvlozj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sphnxzqz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kkvztlrz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3yrsztqow.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3odtfztxz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3emxrmpjx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dnnmvqqe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3byvbiobb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fxenponr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqfruxh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iethdkgy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ijcxkiwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zecexbll.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vueuqwxb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nbisrwmo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3htnjzead.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nhkdhxul.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wmjreeku.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mmrawizs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sbkprkdo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vvyvdsfb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nkadnlxn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmhwapdp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xcsosyio.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qgavicui.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bgvzjuak.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3awxoxnpd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fcvczaod.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mxlighvr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ewwlwmct.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lolpiksq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3trltogls.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wmblbyys.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jwtcnsnb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnxrfis.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tcizdnoh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3slcgbznr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pllkwzwb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yqcgbzqa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3exsofkho.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mraszhpq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lovleecx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qfsctxkz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qjhehulg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kiqhltgj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pwzedpge.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mghsycvv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3sbyzztlo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmbljrx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nqpbccjl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gjofznjo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fsqcccad.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kkmjfpbe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3yomouysw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sbkwyfmb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ekqwntdr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uidncohr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mrtokwpc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hhixippy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xtcwttfq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nzqtdziy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tatayygy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pngewhak.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wxyqbyrb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lbsamclt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tzmkuprb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hkujlauv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3prdzkdka.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3csaogqfy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vbqyidqf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ohlsfiym.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3axfkhbcl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cotouzef.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmmkrlnl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3crgedxsf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ntezihuj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xtgtcezt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lxzomdja.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nxdfhmob.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3umluqrud.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbtvqget.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ipuxqonk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3asxsvuyn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ixjbbveh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fcdogzyw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cakaecmc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3roaxxpzi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qgfkyjyf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3effsfdlo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lasczblj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gfqoaspr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pwrvdpwi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vgrryguk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xkzdgztr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fkrrmsfb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yevbnzet.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hdchyrwr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3phhslluk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwicdqr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ofxtmnnm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zietwrlv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmjkokrr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lxeizeeh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3yddxtuns.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ctzapqoi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3chskinlq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nqqhbabr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3iwmpezue.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mqzeqlnj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nsfykvsk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3urmntokm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rztdyztc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3chgkipxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwlvdbe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gglucqyz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjaitqkm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ygmathmt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bdficgum.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fayjlimn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3iquzbopc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3goritjqm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqgtowu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzsigdab.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ebzstnch.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3flcejxnc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3luxeifzm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lnbxknzk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pbqcavbm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ctgkfwil.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rvgvqexm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nxxuqbgz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3oqabocnq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tsdkodrn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bfeyvjsy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rcnnbwnw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hwmjcrzg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ktfqndke.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjryxpqh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zzewvtyt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jfhybwhy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rzirpdjd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tpzijapd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gwxtoqsv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bdtsmqtk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nflpvnjb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yajcqelc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gibdyurm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ymnjjhca.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mbpropnb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yphwqfqm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3sdgcawmz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pniowdtr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bqedvasp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qnvougxp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rvwfmzky.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vzsyaopd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3arrqmfsb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wlpffoko.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gjcvnwnp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3oghkgoka.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3oraftkgm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3sfuwkgro.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibsmvegl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kumdcgtb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftbzriag.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqgbletb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hqnryhti.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qhtbjwgi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cbxrjisl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lgloznnr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3umzrlgis.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3loqltgdj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sozhszbf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ygvpnayl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rrxxgsmn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xzwwzffi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3upuwunis.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xxwrbydk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bohdyavo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oztpyjtl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xslapwaf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qhoxtpoh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3efvmbqbx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wilhzoaz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhzdjick.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rytitvye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnqpltym.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ccbqgmxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqgcbtry.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3grvsxfcy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3yvlqtocg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ehxegoqd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gmdcudxu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tnsliywa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwyewngw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ueavihds.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kexbmgpi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zckyivtt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qyaifgrw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3awfcrrkn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3adqwryhr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdfpvswb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fkxmsibx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kxfbtxwn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ejsnbiqp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wdbqkfga.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3eozhvuaj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3byxcdxpm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3trsrmicl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zsxkheya.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hsbrocyw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jkfcaxpw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mpmcysnx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3psiqqvye.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vmqiljtr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tulumpwu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wyqxdkur.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wigaypuz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fshdwkop.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fulrpdab.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nismvurq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rsyeifof.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uzlazqxu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ilaakpoy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ycwxgnsg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yqlptade.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3obyquyde.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rjatitkd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eceqxfyn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckhussja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fzmbnfij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdbzhgx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hemyhnft.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kigiolav.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptqxxiuj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnmtrtje.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kzivapss.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqpwmdcg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmgofnsi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3crtpbqdv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3osmkzahi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rncnumyu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zuoekzpt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xuascnbd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rrzyfhzz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qbjfreae.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wmzhrzhx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fupsftvm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nalpeyip.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3dtvbfgpo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ytmnzbay.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ocmpdavb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tjeoknly.html


<!-- 参考信息 -->