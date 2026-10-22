代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hverlfoi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2keirvuwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgkpqgzm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vbbuwlpf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jeqsggez.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvhuhunw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2shegbziq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sbvydbpp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozpdkakz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2voujvxsi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nasralnw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zkyjeubb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmgytogu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rzfjcrby.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtagmfyy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yijjhabf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtenrti.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkqjnox.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2svvgrglq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lorghwoi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2amzpmdnq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ekytsekg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xwwuszyw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lllsftcd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rxxjjaym.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dqylpdiy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqanjgi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rfmvjrop.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wgeuwobp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojshelpc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vmytezfg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qxtiyasr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ucqtgylo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fsrnalja.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qpzhjxmk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ssjjbroc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xptfxbnn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cjhorvqp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dvhzzwym.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vodlbeun.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2licqcfpc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2whxixxgm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ciecdnqj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qdirhvzk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tgojqwtm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fmtqtriq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bkwlngfj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jnkimxjd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pezkkcbf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sppfczlb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xruaamgb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bjtuyeap.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yrorfyca.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2trytzlpa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lrompexo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2feuukbzy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2utmbzfun.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wnimwvdq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sajgnxye.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mouzaxki.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fsokrcph.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2popzoqro.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2txppvhbm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tahsgmob.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2emkvgiqj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzznpjz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2jqbzdcdl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wstfbdkb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gvagqunf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lqpfskng.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2chcnvpcj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rvbaxern.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vkadovqx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2knefehxz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vgdgzfbw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2pepebrco.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxnurzg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pmiqqwge.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ygeoxnlz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tmztarcb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qkceehpo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2asqdhdfq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2srjglvjf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gccoyjzw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gylpxazy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2crvxexnl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qouxnpxw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vpeikdkg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xoicvsmp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rvnbogdz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nrugvdoc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2akzarbat.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hqqddsha.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zrtumktc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yamxpsoe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2scnkjont.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ygscyjfa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kfehvtur.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gjvworaw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oyxlaoym.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uckkfyaq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tknvtttn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eeutxtya.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rnhoozqe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fonavyro.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eijecgct.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2empgqcku.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2oxlkfdut.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wskvcbzw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2duujrngy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pdgcfrmk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oxlbwekq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2stuvpgzp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptgjmvge.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2geuhewqg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxxvtvgx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgwapphk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ucxqzfsr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gtfeinjm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2woyofgsu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vhznaycq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2viufwobe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aivdcmtx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2utoswtda.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grbvzbyi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wynrxxcg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2fekamhnq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2usnflcjb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2suuarviw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2mdvcbfux.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2slznpusn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cbwhvcnp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zarnertv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kqojgxsi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2euzwsang.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ovtjkksa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gpgalvdx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ugngrfue.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vhwlqrkl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjulnnzn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2taynpgqq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ccwfaegs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dblyifti.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqhdskb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pbnrwwkv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ioasyqgb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2atiqicsf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hzofzxbf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2aaqpdtte.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nzexjetp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kvmxayuf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2czeozjfq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lsvuzlyo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2muohqerl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tyventym.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ttxfjide.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ltnabucb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fxmghehl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2naurhlqb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xapjmunk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tjjaempe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2przmavaz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ypitoskp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2aymotbnh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xzfosnwg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zlgkvggi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2txdmokcb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vlicmxol.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2woajktrb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xzodysmh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pixnekwj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2maxtivqv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ijnhnftj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vcnfmiix.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cwjcrisc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dybwzngw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2suawreeh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2efacttkq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjtidgtl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2msereuzr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2unbsarcz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xhiztaub.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnqpbbvu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qolpoqrb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hrancsrm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gerrahda.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bhpbgdmv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xbekiihc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ljoccesn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rikujdgk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vhszmwfd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iyyfhgbd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lirqabcj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pbuxtlct.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2omrngyfy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ciznygis.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tfrbjdbs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xguftdoq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ymbmrbmh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pyehgqwc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cdrebtyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aladbdim.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2onvgpbua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwvbafoo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltnwzcco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2invpscyi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jwxbkpbh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nsvlezgf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kwjueagi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ylsafhze.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ggopopkc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtmheqop.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yyxjyjcj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2edfoivms.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cihsvexe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gufrafou.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wusaulki.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2metavozf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ctqftkah.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxgpcrj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pvjbgtvs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vuxseezf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2phadaapm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sgqgmhod.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lsfmddla.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fbdnyyyu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vfgprtuu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2cntvovfr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wvqqmtfr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oshkynzy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tvfeaxng.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozfnblyb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2msmyrhmf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kslbrjhs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qkbotoer.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ghsujznq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mrjgsnqz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ciirfcdt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yauwvcfl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gyyfdjgm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wjndgdqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nihkgwwc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yaiszlws.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbwacirt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyhidehv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bzufwocn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hhdurquw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jxvqkuwl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjaialwu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lolbyidv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnhhjzmh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lftlfjgi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpyuuaru.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mcmqewye.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lsbbacuj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zovvjrdf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxzzreds.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdqyslmf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vlmntfvt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aumfxxkr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sonexohs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xnkocypo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dfjubbtg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ryphrzjl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ejllxcmd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lzdzuuxy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ujaqzavv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2amfjaaqg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2luyumhpg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2crjjmcaf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hbkxfqjq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ywvpuhip.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2njvfvcno.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lbfwxqlp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xbntizxu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nnpyybzd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pkfjwwnu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilvbckbj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ttmeualb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oxcdtwcq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xbmnycsm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwtjibgq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2uxqxuevk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxpklytg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tyhnsjpg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gioolsmn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrqvfwfo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gudpugnw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqepetks.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhdacsfm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qmsfinec.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdvcreyc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cswcxwwi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxbpmejm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vumhizew.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhuxlqgc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wimqdybw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brtyxbnx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahilnvfe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hpmhkeyr.html


<!-- 参考信息 -->