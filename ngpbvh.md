代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wjejsdhe.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mvmjpegz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqkadias.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ktujffxh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qgwwaago.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vmwvoblh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2awphxblh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oluquiuk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmiojso.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bmuczadk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aylxuhql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xlanbeov.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kjoikgjy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2odwnuttc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vfzgrsjy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xbqbuxsg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2chlmlxuy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmppemn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xuobgppf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zeoovkof.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2grjlvcao.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wnxuhuew.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ncarmodt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rmvugtco.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2necibyjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ldrhjkkd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qmjoidxo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2htvxzmdw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pcqwtbut.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2coewadwq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ehhnlvjw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmoucngm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ntmlmnje.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggxosjyx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jhaexskd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zoqkkxmr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jsxfszys.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zgatqwbz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2slqhbqkz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oxficixk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cpenbnka.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yhrttzoe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zfhsdwrq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yuqifalt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ctunjebc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ximqabtp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ghewcags.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2epjlcnml.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gchwlnid.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qjlcrykv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rieamtax.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bacrkqoz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hefogdfs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uuitcdyf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kwerddew.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzyczpj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gnqyokck.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dmgivfye.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uaoagvmj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fyqwvggs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mjvkmscw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2oqynolqg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jeqbycxr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zeastxbh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kxpkqotm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2celytfsi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qozizook.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2srjoekpy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jjywojxj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2otazppva.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2slglpeqm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vxabzpov.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xmhhbwsx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgbkovm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cpcuokeu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lueyysrs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vlkprmki.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bkpnujuz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2krvkabyr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oisifibh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yyvqpaoo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xupvdlfj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ceugysmd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2petrwurn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qscfuign.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2asuliwme.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zedgqbtm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kjggxpsc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pcgnvwxv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bpdamyjn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2efqvnqal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dgxetayq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rtomgbjz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rusgnykh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2aajulzcw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qdoevqru.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvapiwk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hjmzcqod.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftziyanp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2opecrsmv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhhjdgcp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iklsfrhb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gufumavb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rcctvalw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tavpnqca.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wgysnyxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2igwzpbqu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wthayuus.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dqxfkiqf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwkesiw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hwrvnvfw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tgsqrjqj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pldujesc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wpzuwnrt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fkkgsszv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2udwxsnxw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdctxdjg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lfzdouam.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2enhcwpod.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpaqskpf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cdkbdyer.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2aomvulog.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vexnbgxv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xtvorlfj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxsthdr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fgztxunn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tbsupvme.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kxpooeik.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2opswumxt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wtbawaca.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2osnatrpm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yroibuhk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pymfbgnt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zdpovxlj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2okzhyjjx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcjjicpd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyewtxwv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gzjfwnkc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2psqkmqhs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xvmbfhzv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wbxnvuqn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2crglcnvt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lviynlwd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rcxmajzw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hnjtencd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xloglafm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ddbgxsaz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tipcjluu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lwwkacos.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dtzknzeu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hjjcapcn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2orudpqeo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rvndzvgx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xscltdjk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2krpexpfi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bmwiiazu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yinimvly.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lwkphgpl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rogzcwfj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ebpwvzrt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rzalksmr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apxgelpb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsqditkd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ppgzqulj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymxmfvly.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rsykweeh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2oqcpddpg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2byrwclzr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dplrneyl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kzzcvltj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vtgtzopb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ziapptsh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xyhphzyg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rjcpcxer.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pppgbund.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nyvaptkx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rwlvraoy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2izobqodv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zjnjejas.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oiyvuugv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ythatxcp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2whyfkhoi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ivcaahke.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ottksjmq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bptazbow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hljurqdq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mrbhlnqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fklwdbww.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2aialdbkw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fdvtllsm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aomkegom.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ybktfsgm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2animetgx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rppcbjwd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mpresiuf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhjwjile.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uptpyrmq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vdekwdlo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2stjfsvwe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zaunaazr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tsiekgug.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ssiwqmgc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qldkomio.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2icsafsbj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rnaxnejb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qamuypnx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mhhpspag.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2svpkfesg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pwzfkklz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ytvhzxrl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hmambvhd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jgjhpcsu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bscdtdpr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mzgngljs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qsgucnkv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bkaazxqz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tifokprv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vcbzayrs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yrlwcxzp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wchyjhzf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qcynkivx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hiiwnvbj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hcnsbsfq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2luteajih.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mavclmmk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vqvxfyzq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ugsoucnr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mntkncoa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqeovxqj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qjczrzpu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2biklaenj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhfmaemx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2waaojfpo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkrvjweu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltngfuub.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2flccdrks.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rokgnltw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnsiwafw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kwjzldds.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbpgqdmb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cujzausk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wikgsrjc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kipfsuuu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lxoxovra.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nkirlvtt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bpbyyxtr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xwpvkdna.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qwgurnmi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cvttudsw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ursfceug.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uoayxoyq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2pqbeaqpv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fipbykfk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxdzifde.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eizuvxsn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tyhvqkmi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qawdlwix.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ntelidez.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lzwovieb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nyejlkbt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2idevviul.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qazdbjaj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2svdkipht.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tibehdvp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fhgrxwfg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2arfkuqxc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tbqiaetg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvqdkrsy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vpvhbqom.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2omajyzur.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfsutfyv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tftubuqa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgevszpu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwwjrmvx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2esbcypym.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uykiwbti.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okbzwjhr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qkvmvfdj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nodomywz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiashjbf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfgcciot.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrxtkwea.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2taymjxbi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jbhuoynw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kxkbauie.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdadenqg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pydsugye.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jhkltlny.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrghfkq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xpaxoggj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fshwalvp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zkgkgpsm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ubujecqb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ndvjiqot.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2udumsvfl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mtzvperp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fiuezcrp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2agbiieyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsjbnacg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uiuhbyeo.html


<!-- 参考信息 -->