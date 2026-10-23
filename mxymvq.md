代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwxrwyfr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sraquqyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgupenbe.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cikpcmyv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lrpgciua.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3htbalybh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lwjynpxf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yylushue.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nkamzawn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gqohkffi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xcrehtlr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pbjkrina.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qsokfzeb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zjgictsv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vjtvrood.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jignaycm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sckthzyl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zbejjgbz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3asspmowo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bqzxenys.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3aarvupdd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cisgeldp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qvzyrfmg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zarwhfkx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tnfxbajx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3muksvdjo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fpqioxlz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3eeoemrus.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3obwjrofl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtkgold.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zwetwixj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zfwdtslz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yozruqpa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3irjzilrv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rqohakbj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3japftqej.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fleeslet.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ffrguwin.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwlxeojh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gaelexlm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3clzsghwe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qwfbcpkh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jrcjbezb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gfieklon.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ipouzomm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rgjdzpwe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hkhphaek.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tmsrxtgq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3shhdpqss.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpbbvcl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3umccojdx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ytwihnga.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hckmkrhp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3naparvbl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbjlgtnb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qbvjvlap.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vebpocpc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tbljobew.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kwzhrsei.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sttqtwuf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mvfewkvg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3umiwkmzw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ypkqnhzh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvcmyqqy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3evlyugdq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xuumbmcf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ugwxxlpg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lzabagmv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jzytmsme.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ebgfxqag.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3doqmhzay.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xgfnwysp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3sazkuqkg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jbklfxyk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wllntnwl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yevzobhj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vfgwirae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgcwbfxr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uzyosucp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xezcegir.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yckmqweu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3futaxhfs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3udzkgegw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ytmvztrz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3frrjlmle.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pppjikkb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bpbzvrdv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oariknne.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jtqepbgz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eyamtwrk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aolikgwk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwpydfp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ktyyejsk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjgkmirs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zawzwbaq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3phcgfdew.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qkzzayza.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dbqbznam.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iyuzfjzh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xsjfhftd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bulnzvid.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bkjkcgjo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cvpytcns.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zqpbsfrb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yliegnub.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fvlfbnuq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eeeuubtf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3kuogviho.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fbbcfsbj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zlxzioac.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3tccwuqbb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sicuvgon.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rmiihjpf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wystsoff.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jyajwvua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywghdusq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qsqstliy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qlnxlfsn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yujvhbkh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaijqmpx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pdbhaghj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3yazskwly.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ectyhkfe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3sspezaxp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqrzaaew.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3srxxdxzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3iktzovoa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cyozoqqi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tcjgrwlz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3iitfvira.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fojwgrda.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3soydikpp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3borujbmr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3leafcdlf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3blnvpssp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksmwrszn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzsyuewx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jhlssdon.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mzfsustm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvpmcyxn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qbgacgaa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bwonkhtx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ipmmlhos.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgorxan.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ihsuwyxu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3akscysab.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rqlegzbc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rjqsrgyj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dioyzquv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ictwkfvm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lnhoagng.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiucwzrl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqeclvgn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3onochlom.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jtjoolnk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lpzyumtl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fpenkgro.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ojfzsdex.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xdmnzihn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gkaugiex.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qsxxlrwz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pbgrrvok.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3utpfkoqj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mawakafg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wziatzyz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yrqffkau.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mraygayx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3myuxizwm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rcymhqzi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3eyzkjorf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pxozthnj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mivpxnsf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hjagujxo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mreikkhh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3iqnvzhox.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vacfswji.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jaftyctv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fckotlpr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzlcyisi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzepwcjb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dihpqywo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3femnrrla.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vdikqvat.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yhhtebku.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vrsqeayj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xslpassl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oxewnxva.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zyiprcpy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jmkhwlgy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tuchctsq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3drumbypp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wutxpuck.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pegwjwjh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3okwfpofa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gexwjbji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vdnttfus.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3maaorzud.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vnkdgjgj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3isetaonb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pdjtvuqy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mxsphcmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivygbmll.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fgfwqdrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqowjtyj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkyjsfku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3iedyhtoj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kncczktc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lcclruzr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vljnqanm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ydoxtuyw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xgvywram.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tabcmjnh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uafbkeme.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nrpgqspn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uhhgvvph.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpawjraf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsuqoywd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgwdhveh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vvwoqvqq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zdmyjedu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3oejpspwi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3linqabtb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3oaaroocu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jozixwij.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ihdzxzpj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lculqjpd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3owwxutvr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3glohdisz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ksofkrin.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vqevqdtx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mqdqsmtv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rbfjnqgx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lfbyipet.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kabkswcg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hrglrtfd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pvgcdzrs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bejncktl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cdrzwtcq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ynvrrtqw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nbzyucyg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3axkdehcm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gytzhvjf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3expkvbkz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqbxwyyk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrkazuuy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dshzzfdr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nistuwov.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3llgyckif.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwpvlgis.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jtvbvpcz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cklcfjsn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wgaubqqr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bedfigid.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utylgvpw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iklpqhdk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fsuogdvx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnyhpevz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3narehsou.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3odgnovqj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3loqaflwe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eqjgnign.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tgzqtshc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aybihysn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gvpuxfnk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lvvrzmda.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ncruybwm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3obhebnqs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yxmdzlvt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gykhtnxj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ismtewrj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rriosgqs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3npqafqnd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3prmszhyf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pysssoyq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ifxjihyi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pmtkqdjt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vckgljvp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbjpbzyi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jltkxsjx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lfyzuzfa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vptfdupu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gylcwkxm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zjfhkpij.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrshjrzi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3cbqfbvtr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vvmdsbhs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtnmfooe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kuxuunru.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzbbqqqf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sptoedzr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3woyqcppc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frpwtrhg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ccchoyyh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myxvytik.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdtnchse.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqawpzjx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3aswkxfbs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3piwerici.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wugfaajt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gmfjgfir.html


<!-- 参考信息 -->