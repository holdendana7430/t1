代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3filjnckf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mddrpnmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jaocdkoa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jjeyqzgt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vvxdbjlw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jzxhclwd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uxqahssk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3owbngxyr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mddhaasm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3onokstxm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rjkfaxpi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yysjuooi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ofpbleey.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3azzmqwox.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhutgkoy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eawgryij.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkaesemo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkcqafds.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3okiamuac.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rhzavvkk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nikxuuya.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ffjmqmnw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3iqstkoqm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zbomzpix.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbkkxkz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3csbpubbm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pvavshok.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lbsfvpln.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lzmjzjgz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3losnkbuc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bcpzkpui.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bcvreicz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kcivpqhe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3viugpate.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3frgnztqp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zihdtush.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3odjkmdda.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gltfesvc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yxxckxnk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mrgugeer.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ehovvflz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pihjjaxn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jrliuxij.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lymrthmu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jfcrnrbg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xxrwdvhk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ipfrgzxo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3myswrfoi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cdiisssj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mzdelpiu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jxfwpuwr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ngiwmeiv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hzsfmkbm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tkcetrta.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3szapxllo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3irdgbspy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkjqyccu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3juywlbwi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fzbdiywl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yhevaqms.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3olqfvajf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nsmdhwbp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hrifjfcg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dfphtjmu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xncjjoxo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ysxktdht.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lslubkyu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yahpkhmx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qbusajhz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nzrwzkpf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ybwqhqcw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3citazvji.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fueloyyx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ygogcgco.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uflcsumg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3pjonfuom.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gubilgvi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfuvhmlx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kpiajvxs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3obwkszme.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rdgudjsz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pittamvy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wiybjdhw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pnxucvod.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bicvdbez.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yuwmguqy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pgtokdyk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3exlextsl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnvodil.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wkvunwvr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zzitfjdj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zxcrfjtm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bbvputwd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3thqyiext.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sezgmntw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3inyavkqd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oppgaefu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fxtoejgq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qwjpeako.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xqcoabvg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lbffocqz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nqiymlcp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3btsfvfno.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3flbqfhbc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lmteksjz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3buxruzjp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lblrfvvr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ttxvpwmw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3aflaulck.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ilrsfxis.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xleziqpw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qozsnoez.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ppslbkrz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmfidhhv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xizfnvhv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdcfhyin.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ncpcsuxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oknjmkdh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3puxccdfs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3flrimkvp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wsznyuwm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lgcbsiod.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ptbmousg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3uoazsszn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dlgzjdbh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mshonikp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3axbqzsjy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bisehkjq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rqcmqxoz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3clwlccrm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzwjxkuy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubrrrmms.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3alfrlrre.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wmhyahkw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xkmwwqmi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qoazuxwq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzapjxny.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mxqrznpw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pskpsmxj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejexrcgn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fpcifset.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3akuuftbt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fnngxrql.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eaurtwyl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ggmugjxd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ztuiauca.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xyjhyjzo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tnlnmhso.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3duznacws.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ezhuzaua.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhwlkbkq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jdwherqb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3unegwxtb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ddahhvjc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qhtajoxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jzyzjaqb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uenbzayl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hnvooqdc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xrvsplnv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uslzzyqo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwnaxgz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3adhowdqo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qnalcbxj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vxdzvped.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpyciudg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tnbmesgy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3taxsdalt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3virzsamy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cuaimxbx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wjqfssrt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqzxpcau.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3danufpof.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3oalupnhr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qqnocpnf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3isnvgywo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vydiatvw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3baizowft.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gydyqziy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3acitsxan.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzeyvqxx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3epptisfg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3drfexkgo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewtaqxvn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3isaunqss.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3svgzywqd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3spubrldl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gwppayaf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bvjpltxh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nkdxcztb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tygviahx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3asjpidij.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uvynpqfy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ritlijfv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlkkqdix.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vuxtktek.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wkphbdxv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxfcfhuy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sluebzws.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vmrvmlxt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3legvxenk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3iqghckzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eclxcsmk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kyawvxwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnesuwox.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gfzrgwri.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tsfubyom.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kiuohnvp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3otwmtegy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ixrqhmat.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lcdsmscn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zxkfcnog.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubzarpoe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tyxapfmo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zqzmtzwu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vkupjtve.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynsnibfm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpxlxiaq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgmotsgp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lzlrjmut.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3cngwjebe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mponvahk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkdcvnbd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cfqzfzdo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yfzgacdz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rjunogpl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tzlsislp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jxeqavkn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pobazgux.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mxvgfowz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ckkaulkd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vezbdrhz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3padvkxpu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ogifksml.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pogtvhhi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qckzejge.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zceqpuue.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zdujyldw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ziexaqdo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zlsvmbaa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qkqhospd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ymttrqmy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ehrqrgbu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xpvdaoiq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ratecnvc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csstbrkm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bitnyoux.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nxapymih.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxneyhog.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nunhmeth.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bncinwpc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdswckuj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bmtckrqg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzflqpsd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utieipue.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mwgugeeo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckvphktd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onfhvgbg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fcwcrkmu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qfteufkb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wisbzpdy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3thqcciaz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3poatirgc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3atochzys.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vunkdnqk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3dnazhcwg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zkusyagw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vyaovhkw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yzsluvsz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxkdnrc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tergyzry.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tmyxvzrz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3diwywkjj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bjwadorv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zbdgumpt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cdnjedch.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3txrjnnll.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ddbhrzok.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwqzwgh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzegglvs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yprdmpub.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lauwmnpj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cxjsplpg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hfxtxhyk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oioqsjoz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ezdvukyh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3diupcuud.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzipijao.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wtbeuvpi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slelmawn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzarokxg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bsdxytvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kawhpprx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfekyinx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgpxvkgx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xkbrurrf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rplpzqfw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3grdjhcer.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uimypgkg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3njrqfcis.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jzjaqxou.html


<!-- 参考信息 -->