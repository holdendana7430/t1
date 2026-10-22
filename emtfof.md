代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yuibobzd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2auoyhkek.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lfzpnmgt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2poyripjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otpxjlsi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jvbuwmjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2harhicpl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqjzakhu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lzeivvmq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2uluuqrgb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ubcxovwb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tcajjuka.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2umzyztux.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wgrmlcye.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ptntaahu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qugxvkmv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pbqioifr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2efwczzjp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2araolywp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eolwasui.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2whzeqofz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2axwscdtr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rdagbciw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ihfozdnd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qtplveqt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xuywpxwb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jeupldbf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kdfhczsu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rihtzvfj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjdbeww.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2radvwzdr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fqdtzzhw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wxqqpcnt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pivgntth.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2oqyjvcyl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qavizusv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mxligbau.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcjurcb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xvdnxiep.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ltrtwnog.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hiafrpbm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xovxmlee.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wtshykja.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pjhrzvzo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2pmdkajxp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ykuuucyy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2idpwjiai.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zhfvwyby.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gluoleip.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bbuxyxvd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2uvpytpcg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kncubxxe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ucrbqabb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nuwzjynx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vjttwper.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mqzsqoii.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lftrxacy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2erwjkldw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jleluiid.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xvdrnxrt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ointxzyl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gjwellfh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xzdblrqt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2crzpxcnp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mymxgcxr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wagrcinf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2gupvsizy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yolqqcax.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2cnrpesex.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvxikgt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ghqqfjom.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sifxneoz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2sipgnzna.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lovktjft.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2veyenrbm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eevuzppr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dgnftram.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2reqtdbto.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ejeydfcq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hkgytpjo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xmbpusrv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ryjckcsa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wuuuynhp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kmqiyaxz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nhlfarpn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2izagwzge.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wemqdxmj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nfufnwbg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nurgxpml.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mblxdfef.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sgutyqfo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2neercpqb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2afmbugjt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2baojomeh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kfpuxpkp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2epcvlamm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bmxtifno.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2twmvzjae.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cyyxsciq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jdegjvxz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2npwuyqgd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2upxktamu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nvsveyxf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pckpnvmg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vsbaopxn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2emmgkqql.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mrkmtuim.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aesajzcj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pepscwjt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2voriiqkv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jyfxtmxm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nijcpsgd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nckynebt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lmrcjbrv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wohuznko.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2htwqxyef.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ettfygim.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vzyselnl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwdklfxj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wcroftrv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hddlljwk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iytfwgaq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sqlcqbsq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwuqtzca.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cqlrrmnv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zkaouupk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzvpbafj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vzhsmulj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnxaxym.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vbstwlaw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ygrpcuvm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bhtfbmmy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvpukwm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2aipazann.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obdvejst.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wbqgahqj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2iyrncxar.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pfjnasfl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sdweyzww.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eimvvync.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhrmvzoh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdylwciy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fbwmmtyn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wltdhnkj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kxbbascw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2daveanru.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nummveka.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kvenivzp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vcjemrtd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2cmenfspa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ljnhulqr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xaftjnwp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ypxrcrbg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vdoyaulb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqnprgfu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aowzbyyf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zpxygngp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nykdqgls.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lvduiwpp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gmrzntrz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mgpsogwo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2temabgyl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cfeomfyb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oyqguaho.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xytbtzrr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lmmqthle.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dytycsku.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwwfypeq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2viqstceu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dwziukpp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gqrfului.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wvueewae.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvzxuyw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nfycdssv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fafvaqrp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bngmekwo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xwoypcvf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lsadingt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ddqmnule.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pgeuyofh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fhsfdanl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2doigdmcr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vedwmhmv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2atqeikhm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewddhckx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mesykbhg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qtgythnu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zgvswttb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nouanjwt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gfciirfl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2igqureio.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rqglfrwj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2russbfgk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ptacdzqu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mzjgfkpn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tylkburt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cccripwm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zfyftwkq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2txsyujbo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sdothzbn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dmwrmszq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sbbiurij.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2awvftifl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ucaujubx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vwjdpivj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsqimgbq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vemzxzsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnqvqcgo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpryplyz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nrdbrnpr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aetacwok.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wwgeslzr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vkiqhyuz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tvdmihzp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wfkrsfgg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hysskhvx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iyxqawrd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jxvjnyqy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tocovczm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kstrrfzc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zhcfzegj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhlpexbu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lpnmcbjy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmvkrtx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fpbgzwvz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2avoscgcs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2izpbjtkp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vuqzmdrs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ffcauycr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hvqoczlq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vusnpuvj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2cfhuayzl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2codwegsy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qzmewqws.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2farjhiab.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxygfqpd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xlrxgytb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ezlxhwuu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2watzokes.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wfjiuyll.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2spmnqseh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2knbfqyjg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxdsvwip.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xazehjoe.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ebuidbzr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2uhoofofu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hdebiebs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpazfcoe.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dphbjdrb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pmpfenfw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dgqjcyev.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwbyrgbb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bopjmbzk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ruouhzdf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiyqhvga.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xalyadlt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyntvtcu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gquycroh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qajggriu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bzhdpmcx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnjxgzsv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kjtukhmr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jdouyldg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rbftktig.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yhxbrqxh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lyneelhw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kjmzrkby.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eavvzujh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vwdxjswn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2prsbmbci.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jtcyzorm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zvisfpbr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lxxfsspc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2epxesutm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2befayntj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mxytsrtf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2blzdpibg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gofqpdim.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wztidxuz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2pdpqjghd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tpxbpjth.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llckoyzc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2restmpzh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nezudkxy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pbakfutq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gkiozjqp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2awthwyfx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdmcqsta.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2whvoaatg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sikmptbp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wloejlru.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fjmnbhif.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzsylpld.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whphvxnj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hrhgnjhd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlvvkutq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdkbbwtn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcntvguw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2luzkoxcu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zccyicmw.html


<!-- 参考信息 -->