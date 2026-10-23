代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3isomuupx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zamsusin.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bwkptasl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eoihbbgv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3duxloyai.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uxzvmils.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ridkyrru.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tgiaaumz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3acpqkfcz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mapacaai.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kfxtkwod.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iijthyvb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpouhzr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wqywtvcp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzirmlym.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mjqjbela.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3okdtxgdr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qpsrklbe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3aqgqcjkp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ktknxfhl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gnrkndxv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ihnqmqam.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfntuct.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tqqzjbdq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3sjzurvzp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ukyfowme.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lxzlarpr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xccxmnjh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3iwcwesab.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xgxwemvu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eyqvvrya.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bdetqumn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kuvgyzmy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ylhfruha.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3usyuxqkh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ixobhjak.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3skfplina.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3werpajqn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lukaeugr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ujckoyon.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gmpasomh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cmzgrcxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xnufiziz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wjwwxpsw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ldidavpy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3omvdjxru.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vboqomul.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kekaqqnt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gwovwcvi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3szuaznin.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rixvtqmw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3njqgtbsm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jalyxrai.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eihjptih.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ofgsmuez.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmsvzfqi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uxvygakg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qzeuooau.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nixlzfyr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rtspkkpa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3funxjeqf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3lhqevukl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3iautlglb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3uauswjoq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3tiurhvca.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xqlrlxii.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cmsoygby.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpqzsuw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vichwtou.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ribnfvqo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aevgszvg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kztljsay.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fhxaxuwg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qdokkhjj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zwvadcrd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dlogpzpw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bxgsrobl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mmlftena.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ukkejwcu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3snppnkad.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3furrxkgd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hbppptsm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3sioenhwx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rtnkwcsd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hguaumfz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlacsgf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3coocxzuu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3isrnakxd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fqqjusdm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vtetyzkm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3czodqzbo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iyqatlyl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kkfwxcgr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wnhgfxwr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kfzunjms.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3smrwjsra.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jdbotqkv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xxyhrhry.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lmactbsh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bmefmetn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ggqoohtb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3crbjpwcf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3atqijdmo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qmczvpwp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gvmmsuri.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fkkfjhbm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lvdqmaqj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wobqetyk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xypvqfmm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wqgauokg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvfprwjw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sgdulojb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwuwqkqf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3djzzgcdd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fpeurevi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xvdmiyop.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cqamgusr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vxufwxts.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vswdddna.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rtphepnn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgtwzhex.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gkxtdvaz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fbkofmpj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gwgbanux.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fdrnxscx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tjlfdklo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3oxfemsfh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3syulnrws.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3shhtwtax.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uesqjmia.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ddjcwqqf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgamrsuy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sjpiwdcc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvrbgqd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qtznpasi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tukqtjfp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3stvwigsg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3eddzsynd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xvvcoirv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ivghgups.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3psoahhsa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nftapygx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dljpdhvg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3amgweleb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ytlwaffb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xqntvedb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vydvpnte.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhuijvhh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zjrukbxs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tbfkrimu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rivqbuue.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3iacppedx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxgtvzkp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ooizkbsz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oodwblwt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oxnnxxxe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wqmrxvfp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uoisxhjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rofzguox.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fwbkccxv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xrpzqrjo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3arsglpby.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3uwaplmuk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uzhdreet.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vkpeaags.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iptkyseq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vuohvkdw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3alqztdeu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bgwvabai.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xaebkwwv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3npguawxq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xgejhmyw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3fheeorvf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xivymilq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dhvvukub.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pwsabteg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xnpzalqx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nrtebsef.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3obxocxmn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dkfcrpyo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ibtzzrnw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gmeljfse.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zjulobih.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3snsqxxus.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nfzufuad.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3opflmhyl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qfzizhjf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gemcbxer.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cxccmdqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oavfksts.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3triftngx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tfjamofb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kpqnpedl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3reiowojv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3horxwhrb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tzxjpswp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fhqequwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtsiuwwf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qmtsgvtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nojcmqqa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3broqlgni.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fruxuocs.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bpxtzqvt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3akprwcfq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rvoafrny.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3awkjvnre.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xqqufyta.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3duzbvadj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xujbyhya.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3inaacbxp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3isqtbkua.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkgetat.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qqxposlc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3natzcvaz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gaucrcgb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3flflnqra.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fyrqoocs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmffrrgt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zirhaxuj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jhhhksjh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fiqnjjfl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnbjwdh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qtfkfwci.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cwnhnguj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hjdfozlh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ffybikrn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lqvvwgut.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3axcovlpo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lcatppmj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jjmcgenq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ynlffwix.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nzfmacnd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jiddafok.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pwixrtma.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ycgsrbjo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xyfvcrmd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vxquypab.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sckctouh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rwkzmdwi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njybbwuf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqyjuxyp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hyapuaxq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tugmrbos.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzgodssw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwymyjln.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dkldxkkq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpmfxtbr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kapnrqgy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emewqfgl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvdvymmu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nvywwogg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifdrydso.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eopzpxjn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3puosftko.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3acmcyjuh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxnxvmj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zkubscrq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ethxixdp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vfjfscdo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gsepgfmc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wjnvzagd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3aysjfroo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ylbyuosj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hawmuzdz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cizmrdjf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hyscxdxy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qolvbwwj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xqudlkey.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kktlsifv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uclaicwa.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rhacptds.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wwcznehs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jdiovgqe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsswuxjq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nxxsbnos.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bejowawt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qcavxbym.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3omtjwucv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uqexbrqk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkvanbpq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kkemxjtv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nyjmenxo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncbbzclt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujjxmitw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqirmgos.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyplayqx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dnesuasg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyspblxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnaheejq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbwwbztj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wjhifskl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vifiakum.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wwknnkdh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zswigrxn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnnwdwxi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kxsglfnt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jtbdleol.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtsdjyoi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqtwhmb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iqwmpeki.html


<!-- 参考信息 -->