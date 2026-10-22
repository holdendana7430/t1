代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aykivtju.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qaxlapec.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2apoxargq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rfeuikyl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2chedflgh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2btjryxdm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2llyhmrqk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gormpvfu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rtyqyfko.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vwczwrxp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jbsukcjm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vwnoqoyu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zcrovnza.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vreuyeml.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2juwyhblu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2stevcjmu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2pefyvpwq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tclgijei.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2olnnkxdv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kstkvuus.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2indldqof.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vsqysoso.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2whsoolae.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nstwjwjy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2upyppcxq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ikztmkcm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fmnmpujq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xmybvwzf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qroqdleb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ydmutpdy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2korqvtcq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gtyyjfdq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xgybgyla.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rxpaouzv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lltdlsmf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lkhufkdk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2djjuavgi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dmcruhqj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2klokqcvy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2szdpoacr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dwvcoalv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2arjhspms.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrwxmuh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnbdxfc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ekhhwwtj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2owhkrqce.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vjnplnup.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2boyebyea.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dkiyhugt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qjfpaoow.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bpfwrpjv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nimfertz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yijdxzkb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2erumppyc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2msjnvgpj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wefiydqi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvhfhoup.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lcjxxqnv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2akwohaks.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yainhvlp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jbzyaqre.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ddzzkskp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xqdukjpy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gfmgwylw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vophjscc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jlvxxxyb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mlfjgypo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kdvduuts.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ngmtpmgr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sthybsbt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rkugzjnl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wyvufvrk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2apiodval.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvuhvafo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dpqkaycs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iuctzwyx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yjlmyfqc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lzxuanqr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2emuurloc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zlgdsiqr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xafdxtux.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ztwgndnk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kewdcjuv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kbekttsd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vmcrzwks.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eqyvbwcy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bhzjhhra.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ctbszoek.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vxymroae.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cqdzgrpv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2eycdctqi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mjtfsbpn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hzsrqfno.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2cwviezav.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uogtedly.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmceynst.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2crtwpqbj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cikppjoo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qcffwenc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewewfqfz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gtstnlxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2plkldfkc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bkctgjpw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qcoqoean.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgiobfwx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wpcdzmit.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2msqlaqza.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cupxffff.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nknzrqrt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sgppouoh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bibgllnl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gomzgqlz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxlbwwr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fkzgaawp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lrbykwnp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wulrtprq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2sfxqwkmg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlrmfhvc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xjbjduie.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dpovbesi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vmmdxqcl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vcyvwuuj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jurjcxmc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aghsmhbv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2acizabld.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2scjeqtmn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vfguduvw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2onkcfajr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kpoexhks.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnpasaoy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mxgzfqzi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2douvfygl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2elyjisjr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oetynoyn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ccrvvlzy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xwtkyeho.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qsfhjkhc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wtgphaue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tnmywgkf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdxlczq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2divpqkwt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2txislftu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tkranbqx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2umjxgrfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wtqhzduv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2aduybesm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2snphpeve.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hunkfeat.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yiyvplup.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vimtjnbv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahmlfggk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ugsfusnw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nqjyrdqg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vuyptdqs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vnlfiqnd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xtfhzgfz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hatnktau.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vlqxelsp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qglraywr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zimwbuwc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gmggxnnc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cvxduucc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tcphljvu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zeuachva.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aeyilwml.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ozeecjht.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lyaeuhdc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vubobhce.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gsuwrqnq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bkprmqnv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rwwssiqi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ytbhnkdt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sudqfhta.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkxanlgy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vmvhdjsf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vugljcsw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmfjchir.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sguaviym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mnyureds.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qnrcyfze.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nhrksrfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtusfdxl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lkrotnyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qasiygta.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zeufwavr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qhjxtegp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ynhlapsk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zbndjxqw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cuzqhmsn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2umpbirsi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tonmdwiz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jucdmlpe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yadkoihi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2bomwkjrl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ykddppeo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtqwdtks.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ehmbdexr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smfrtttg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bsrycchi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rimvgkoz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yqosyraw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2prggcnex.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dqxbyfox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jptoovet.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vojuooid.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fofarwux.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nvuuvxqu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xrhvduil.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsztwcu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gbibnipp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vzpmtgkc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jfbryvbp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dcfpolxw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2topkigvw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vkkoworl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2usbnuvzu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2julznmzr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ihbeqrer.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tcntxxte.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ooamhcev.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2oidosyrl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lrosjznr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2frlucxji.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jibdszmi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbncncan.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfxnnycg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vpmduxke.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqxtekge.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyrgtgmj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kscndqvm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohmonryr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sorqmflz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwsonuxc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikehrepj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nsppsuvd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcbjrarf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzfkfgyi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tyqpjbwl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2umynhzll.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hyxpjuha.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jfqnngrb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fsfheymc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hnriyhdp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wruxnvht.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pffyroqw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bgirohny.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rnnqmfbq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ixajsnlx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dxsnckuw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcqbfqlq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vsmfbjuo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sdnwpqtx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ycqtaven.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qbybazsp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wqzkkcsy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ttyfmofo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2xfiikzah.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubonizoq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rpbizwpi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fkgkmimo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lqbzjdkf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nknxwrna.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2uvzlyhxc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swutwcqo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2njafaveb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ucosmghm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdeolnpc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2crlknnof.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwehuicf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snljuxtd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cpkwlndz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2viepbofu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbbffnvc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdvvmsew.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hhpyisik.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyjtenme.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhiwjmks.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtcfdyiw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xltpjkbk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tskepcsh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vxnbrmyc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2apnevfwa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zpnklpgn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jczdyost.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bmpgwoan.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dpauxtva.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ipvdhbtw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vqjjiwfy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2djuhuriy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2llmjagmu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xhgittyt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jnjlxinq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkhrhunr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2iceuxmmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oixnywdd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2aoosnskt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rwllwwgm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2smhshdql.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrbyljvz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2chggvnkm.html


<!-- 参考信息 -->