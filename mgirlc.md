代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hqwjwczl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3eblhjtbl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ofnwvrnm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fyvxqrvx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qnlfgcrd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wzqpsgld.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kuukqfsx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewhsiqbo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvsfpko.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lqyccqew.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rvuaypzq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bzfztero.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rlownbfv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nbekwnvw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hvvqsmhi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3obecpeim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3idtmjeve.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kiiocyrk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3cbosvtwc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bhoxcrwg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ychnuwra.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhagsst.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uxzqvjxe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gwncdryr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jfojkdij.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xwbyvwcc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pbzpkaaf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hpmquikg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dvhatyba.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3axaybyfa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dpaiwjrk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzxtuvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qritscxk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gpytqpst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejmwqzuu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ogqnwbhd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3aeqnfjri.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xgvgjrue.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qwtvkpul.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yertfqxu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xywyyhxs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3txjywzkb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3eigbwxpq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cgjrgfaz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xsgzylyf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kthvghoe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pvebnlbm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnijswd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvtkdxuc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wzlyyltm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3duzvnuto.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3eeafhgkd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hvcjjbhb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qpacpyhu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ixxorvps.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3whtxzfib.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dpvypgla.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfmxpff.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sknictnm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xpmnzmdp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3waqptgde.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rlqspfhy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nlthwcfm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rluejeli.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kyyuajef.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qlxunfpv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yukavvxj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gxxxpdzg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wcscknwf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sxxqeway.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pnzurtzq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hsjtewmz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qqarctqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dotmkkhd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tjarbtny.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ovmenhdz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ptbqhdac.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jswkvuae.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cuaslsac.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xhydecub.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rvmrhsdk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bxzysrtr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujfzpdyz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eockvjze.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mqjrfptw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hlujzneo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yaajfoob.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pgmathga.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fxkapvkf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3unclkdeu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jilrjzxx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gndyiuwy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xpytcwyr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ruvasqia.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yxmxkwve.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ziijxfgy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3osuqgrlu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tnomrnde.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hkoekimu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3plofbevq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hsxmxitd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3klpzdwec.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3opwcumqo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tbyfmfdl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3iutucwhc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wcnddhkk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kmanepgk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tghuvzpx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybuaqnhj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zuiztxeq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zqjeywbm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3shwoubgr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3teghomol.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lgqzstkx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gcmyevlx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kpgxgxnr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3eqfebwou.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ttyykmkb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jvuyrqqf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kjcjiewv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ydnuovjd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zewpmqrk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wmescqdl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uiczbgzo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bchhmocy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3otuyrenq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bqldvvfk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3syrllrwv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ofnubhoe.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ydbajsuy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rknvmkds.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3npntorwu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rsdjjrvo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nxiuvmsv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pkwqveri.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sabeqbao.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3renzybwr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3myywlxsk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bpcnjesx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ljqnglxo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3clrzuoaz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ejalpxfv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3jazxmmnv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cuuvrfrr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kltvmsmf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vcibffye.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfgbeyyv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nxrjpqda.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gxxnjuey.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gvhgbdfz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rwmbqqxe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbmnwlrl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3dlgjevhp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gpabsmnq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jywwwksl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lwkvqadv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqkkisvw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3odavvwhk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3torbnzsy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ewayrtmc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tqtdsvzp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3eejdsjop.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lrmsvkqg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3plxpiuqc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tgdzdfsj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lcgpyezq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cllvwtse.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvuwvtwv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjpxznc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkujhxk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wxqjbjkd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ygghxnau.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ycermsvf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gnfsyfqx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ifendpia.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ycazvtpp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ejwrutmp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sannfjuh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nukdwnqc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ekuwyfwf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3btywcqfd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cviooruj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gmgdzgmh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwlzmtv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cobyegzd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3urhczckg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bxhuklpw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lapccaae.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qlbwlokf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3riugcgon.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3srcqedmg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zgnsxmmw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jglyayho.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kijiozmq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xpgezlaq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rculokcx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3blwrzkkk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fuyxtuiw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cdesnrnn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3snaioiya.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bshpymfs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdmfgqy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jmtsfxnw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qbojuzvk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3bwugpnhj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cgqqvhrr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3sphcvwkw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cwevgxgt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tzjentbd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3znqreqlo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnrqpbxx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkxrojnc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zbwycbni.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bidbvxym.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sftbubnn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uzouxvlv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gpftdegn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rqkbuocd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sbveoerg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wzcyvncn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fwooaxnl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3omzaerau.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lwqfflxs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gpqkfuxt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3btfmjqly.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhxfqrz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rlgsbcdj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rfmupjnk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxfgcgdl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3usiggziq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hdtonfxr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qagkhzlt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tuthzbvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyfjppvb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3oopmpnzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyhmktcz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucxtrdna.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vlasvnrt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzfeieko.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3omotqndh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bvmpyjef.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3awlrgqiz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3scyvcwox.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvpeofuz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yixlteum.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3epbofdal.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3damjmayh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vdlrfidx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqlgitfq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xlysvmss.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3szdnhznh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbyfoby.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vnptgwth.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkycxidw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uradtyhw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3oqbewcoz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dzvafcub.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bqsprify.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3glsruvvq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wjaclkze.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3njjckutr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3anoigfma.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eodtjecr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3llrwjvar.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xdigogbw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3vembrqcx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3svwzchaf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3junxudln.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pwzveunp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3daofffds.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3klpketmo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mcrmkuos.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3babrsfua.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3daecmqmb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bglzgokl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmuedrvt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cajmdmit.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxrqukpx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fzqqvxvb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emsicbng.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fsvyjbrp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rxfaoppa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxvpasrf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfiocesi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpwczclj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znsiomrm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bkukblpl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adqjvwlu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkkjrrkp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jyhfkwec.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tvjjexjl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vphuwcuk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pdnapasz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oimwghid.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hlsezsaj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3scgeryvr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3pipdjprv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zfpobxpv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ghaipcac.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ecasnrhc.html


<!-- 参考信息 -->