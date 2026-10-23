代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fgipmpln.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3esicsdrc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ukxdykfn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qbflgdow.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hdedrhql.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3iyrtqicw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vvrlojaj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tljrptgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdwitflo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yzqbkoar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyqynexn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3evnebtky.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xbnkwgsm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrnzmsij.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3usqhnwct.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eaikpdtc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qljypble.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dfzccfdq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ygubyvts.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3szhlwsya.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xnxpuppt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fqtcdpoy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ymkyfaek.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3miarsahy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhxptov.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbusslpx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3owspufnh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fzjrokqd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mkzpejhg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jepecmwk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vylqvdgb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gtaiyxxv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lxvsbsjx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ylydiuli.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbaaclhx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sxrvmjvx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rjcpwwzo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pwxtxfiw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sdrohubu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yxmtnjup.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kxmubmyg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rucvfhce.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fvrdwomg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uysaglrg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ioighien.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jfiwmjue.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ipkmxwyo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lrhrurzc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ptqhrhew.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wygngsvo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rmmwhnpk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zfnbgwzt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgshwhs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lagctsak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jualvxee.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iqevnvov.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ommneulr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmuiptzd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbjjqxna.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3alfzcova.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vfdqohnl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3thxjvtdr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3onfnritg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yqbwojtn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tpgqxkew.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ikcvrjhm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hyemkpmn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sxwwztur.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3efomfrxz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hricdhcb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ptixscxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kierhekl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fqvcuinl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zjlcsdos.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cromfzid.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbnpgzs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mgvnfqeq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ponzpcqq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fszrpzoa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rlmoxlfd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lennimcq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cbmrunml.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwikfzc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yslfkyyc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dujvndvf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfzywlsk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3agjwpxls.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hqiglxle.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xcjejkfv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zeychokt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yurpitdn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cbgyvadk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3awbfxryh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qqpggbuk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dptzmjll.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zuzryoay.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eesqkxhb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jgdxarji.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sefzhpye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3taiuhgnw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fqhdmmir.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bbeaqtkn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3igteotzh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hsemtnib.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mlrxyrwk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ybdpiwcg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ugokvtyo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dcjonrmd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qwhbogsb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ifnxibci.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dsqkeufu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ebaybrxt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rutglrih.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aycxuymi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ipgcbeoa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jrlxyvqy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3klspaqcp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3okkduyww.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ahnvceow.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3loepwlhr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ympobxnw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3aftlldsy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcsxxzcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zmdfbriq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mersolht.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tnscakab.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lnrnrgot.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3byjxnumx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3dwuibfdu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3sekojnno.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmuslqie.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3taviwjtr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3difavjxz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmlymje.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3itykxhti.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zmijdmme.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3njvoyzxu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3odauyxfy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yaaeykyb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jaoucfro.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlymdmw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rsoaizlu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gshyhdho.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hvucyuhk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jfpnomin.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sryzfira.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zzyibbbg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwjhuwrt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lugsvisj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bjwlaons.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nuviegfi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rvnyggvv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mjdpnqbm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rieinlww.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ooiqmzja.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ubyyfoif.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lqtcntqi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymrxajmr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nwlvuegf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twenjeli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tcsnvpzl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mumfjtqk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kpgtfdrb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mnjnqqxa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pxxmtqev.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ulsfxmgd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ktvsibsx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qbvbrxtm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3skibgizy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ntequxaz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3unceyuvb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3todchyhi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pnlmuoij.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jxkeblfo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tppwdolp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yxjvlrym.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dlufgsan.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rldtundr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3snegvksk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yswuzktv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jqhlmzmk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wrretjzz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jvbtdzvp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ipcqnmca.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jfxhigsk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qoonycyw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3spfkelzd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eicqyugu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3esqbzxav.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lcpccllt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xohhbsis.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jraxxvjt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ngivwlwp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3imaenqzo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vojylnvj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ewxtnptx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tlfecghp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gukrsszx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cowwfrmi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vnuvjyzo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wywdcokx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwfskvw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vuqopnrw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3btpgfqyq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cnhlnfvp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ilkfdeky.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3oyniasot.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hgzpmqfc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3etvawuru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvigvvjl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3olafwhxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szyivbkx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lpvgvtks.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kehylkww.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hjyuztui.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ezbwxhcu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nvdjzvah.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wixopfit.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3izjzesof.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrcusdpb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3codtbdce.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbxtunyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3brksoipe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3cywndibo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3izeihjbx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkmxnsss.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kukuearo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jqvxntjg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fldqaera.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fbjzpasy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qchgnkwk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mkorxpjv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ixtutbry.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qcxpksdh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fkdlkeud.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3eorewpel.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjeehhp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jemybsqj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hgdimxla.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wobokdrw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jnysbqeq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3aqslknkf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3grtwlspb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jpgvnccd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lctzasai.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tfeciuzu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mvimkqsw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tukmmmkz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fymmsbwj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3myffrcqv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjlcmvyf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxjgkjjw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqjnctkt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dlggvstf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yzybeipj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trcrmbaq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txgdhzar.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwcvnnon.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hblysues.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3snxsrrnk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3otwahwbx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncavkqab.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ddbhddlt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cftiasxk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atvzflxj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjptljmn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xobrqwfo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppqjiqyn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3adpzatii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ykujmimx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3thpzxkrm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lsycwyrt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ilyetjng.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bmmoaeuz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qvmyutjd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xtmtbajy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xcbtmsyo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkxjzmet.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjdnffra.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3onnfagiq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3juamgvaw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3opunjwgm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nmzclssq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3aoxojqlc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3izbiuogg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shjglyxs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gexyuown.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hzoisyqb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uaioiceu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwgecmqm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jnvcnqwz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzsvvqtj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iqcbwaqr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wsygsfsn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgdknfsl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tpztvmhx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3accbqzgs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sproawov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tsdazfih.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlyycawp.html


<!-- 参考信息 -->