代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfrxzhdw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3walwfyta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymechrsd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fqbglhxb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ndckpifz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvbrcgse.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sjgtqfar.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ijvsqbie.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qfvtnoyc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cshyhjsq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tgkcdhch.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mxpkncwp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgheygwm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xdzdiafm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yclabpgo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cqamzfen.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwrxrlhl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oghmzpvq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tsibbiat.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3djbllnfn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3emszmunv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3svprgrez.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pyyomyvp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qgaeuquj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vfobodnk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gonbuytr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ydeyqgtj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3isqzfxji.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wgbyjjvh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fwsoxomu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kvhpfggm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bfpqsstg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3krlevfse.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jphpjgns.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vqcgsnei.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3psykxzuj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ashgtxtr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3alzeggmq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kmhrjoac.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3detjaemn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3quntwucq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3odfdwwys.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xipfpsop.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wwbitsca.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qtrxlnvm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hsrncqkq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lynjtirp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pfhoixhi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3chudmvjl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpwqcrc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kqudszox.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ezdageme.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yjojysuo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fkyxkgst.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3skmaklws.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zuoyihyi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vlzrvtpj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rjwtjujj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ieratdfs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3srnbrdno.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3luqclnmq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tvuhwkhn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wclrelre.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dzzafhjc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vvycshyh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qruuwkpu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3whzvqgex.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3syufvmbp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lflffuxo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cvfwfxqg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jmonzoez.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ftzazdgu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mnvvjlpt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fdggsswc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cucnrnuw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bbkeoaod.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3sixsmjnx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dtwljurc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fjccmjrm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3atevjzod.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tbmigqtl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rxtghvsw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bmizyrpg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xirkqeko.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bbgvmytx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sanqdday.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hlkzgbap.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zcovvmhk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ccndqaun.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3isxtyvrb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3piwyhhpw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eazlmtku.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sjytfcsl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kyxalxww.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nuprsxuh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rqbilzqp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dggrqdvt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yehrckvp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tpymwxzd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nsppzgzq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3chtghtlm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3iwrjciru.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3abiewivw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3irghpvyt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ynnbpucr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ngyzrbig.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gytkphgb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pgqjqrwu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3epspdtpa.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hyvndqzw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3psozjpgu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nrpzqhuv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gftzbroy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdhutejb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhavepip.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ygkxwgpw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ewyznxxs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ykipghht.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wdjphcna.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3slydiggr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hrqpkqfs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kxvdftmq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3shwsohzb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qyytrhvz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tkljylqm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jgjijwjp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gzppypbf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ujhkgbkp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bxficpyi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fqhjpcbq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkysjrx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3lsszjbsy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtmbkni.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tropqudt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bvbtaqxd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bokovryd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unvpntga.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zxkncshp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lgxdpqaw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bnykeiqw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xbtjattt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fmylavua.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tlldcfdj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hjbdkudr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ixhuuuzx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qltfzjdb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jrsbtfue.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jiczodma.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uuvuutjd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3amrjfejc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3whfapopq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcneiaeu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kerccqtb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mknzgpmj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qtxwnrco.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3awxqvtbf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3leqmtlwy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fjzaysnm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3oiiavdql.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bfwouwsc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uhurjwfb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xszfhqsc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wyccpylc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwrcbzfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ryxdzgna.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zmachdne.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3snyfakba.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mnmmoygh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lkvwroum.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbtisqz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rygdwoea.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qbculxzf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kqddinwk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dktcgrwj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nvydpeae.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rqyhdnsz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jrszozcf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vkpgahns.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3absvdqze.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzypyczc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcbiirsd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3njoyfimd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsphfpic.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hfdzzylg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vgetuukh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vufqibul.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vfwzpwld.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jvwuvonw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zypwhekg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3iilemjmg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iqlomoea.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xzixkxhq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wprtvbkc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzvsgpq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3esxworjo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qzmguuvz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ilgrfhud.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cwcypubn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3msdeunco.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yruihyta.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xgqtuxfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icqckrpn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kaizfsle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbgbknfy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxcaufnn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3plgpwlfl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ecajugge.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wwlcnaur.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ybnvilrr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3opllgpqf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dvbdtoob.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uttptmnu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hastlwjj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3labqejbg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3oypojrra.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gfabfplu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lruqhofw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frgezfct.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mwcbcrxu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zeeladku.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jjetkepv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xpwjmgze.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jmwmtned.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3olysdzcv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3stddokuk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fdkvmnli.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dzvdabeq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qrxvhqpa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrzunsm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3whzyrbri.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3flolrgdg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbqeyspw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tgwjyfku.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3cxmqlbdt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3geivwfvm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jpetalnc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vymnwfzu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3upvsoazu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wdpofyil.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xjhtfvqq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wfdwowcb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fleuctty.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hqqrgmoi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ochhedfg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwztavhh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ruclgmmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ltigikdn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfzqtjlv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epuyowsu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xqckpqip.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxouvrbi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qpnuyfgo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sonwsjbv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juovjdjo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xmuphahu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujgqlzrz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxnfdjtd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3geervlwl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3iajvdrxq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dvrxiasz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ojbgqilb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3udnxudwh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wwrdqkyb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qzynsukp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vijlxykv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ltjicbqe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pbmgtjcm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rpxhtrqk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dcnafxrx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tolmqnbq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3himwrfmd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gqwrfsxn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kgfcegii.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jeiwkdtf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shixkarm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3oowlbojs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3enskizlj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbzxlehs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xgnsysek.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jblrdpzy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jzgeysji.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnnoneyo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mdodcarb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqhnicrd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ofzuppmz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mtzygxrz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsinoiqt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wcghmenf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sopbzshf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqeriefd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kbyujuma.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmdooync.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugdzbvlf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhwvzgbu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3moxsxcsu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jaqievbu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twrymyci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzwlvgvn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmijrbtr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vejecxre.html


<!-- 参考信息 -->