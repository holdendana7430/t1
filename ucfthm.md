代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xronfknc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2drwrwokj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2phfrongg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kmlceuip.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mjqjelpc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ufodniqc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ebonrlnc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uekmasyv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qghpidvq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vqexqege.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iqbaehfv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2krlvctzr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nhldatqa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ubpdccrh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lxadhsph.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2zfoohtkp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bsftfhwt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jsyhqdaa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jdvjarbt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jniojftm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kjlisiic.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2oekchlli.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aqpuxpng.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cygoygia.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ggfwjemm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuepipgx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjywkncz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kigfctkn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vdzcosfn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tkzerfrb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxebsuiu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hhexswwr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wdnofivx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vvopiqae.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dggsfafz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2krgvttyj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fseuonsi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sbloagsk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vukkuxvs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzmpmgzf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kojstrrj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zkldfbqq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pbrkfcmw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2eegytjae.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vxwoidow.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xcuqdbcl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2brmrpryd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zzjglkzc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xyuprlrk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nvlxtovq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zafbmlev.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2szbkyryj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtwppiyk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qckpvfma.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ixqlfurz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uehpdxft.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ingifuap.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fcetnyon.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2brdsnkss.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oowaanen.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vmgdnchy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fjxcswhk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pfidqjlz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sxwqskkr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2evxqjfch.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bxeqlzda.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fniyhrez.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2arbyszjo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2eesdyptw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kagejfil.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ilvmelqw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vujlsfgk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2joiatqvy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ervyltco.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2adkzqlac.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jeknegaj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2alocpsyg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2plbjtgno.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2etlyhedf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mnzjrwis.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2iatbagec.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lprqteda.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yazxgzdf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ypjcyvbi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fcuaifuq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gnbthwte.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2efpfybtk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qygyaxhy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zsiarhxs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgfdeema.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ccrvgfni.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hhunqjsu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cwxeesnf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2emsoohmr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2zgajskrv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwtwxuws.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2rbdjrpix.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gejgjenp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aegcckvk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qqzcngpn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zdxdvjpn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fegdgvwy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fawbqfur.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2scpquyaf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fzyoqcsu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xgxnzvuh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rdiavudd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2czrkdgtq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vtztyffi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rnlzphly.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lsxldqmi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbhgelsr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nblzhjgr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2swofimff.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wipmbeas.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2akqkxuvy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qnqtlwup.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bpbdkara.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qjtlfhez.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xqqlntfj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fgetfayo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wdurwiyp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oeecsrpx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mdxsdwta.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rxpdhxra.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uitsmglk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ursudvrq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcsetvvr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxuxwuz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qcsxfrrf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pdjodbzc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jhicuojy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cotcyapl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bicoynha.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gxnwejjc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nkmbzcvv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fnlktdtw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmufobq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2netnqjhe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzqaefbq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bpjmqden.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ruazufju.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ginkltkk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iaoeetvp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ymgwqoug.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bmgqykhc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jmmorywe.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vvksjgnn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sfvhirdb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2euoutwwc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2atrecxkw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2svsgkziu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ugovpopy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzmfrkje.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjienbad.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gjfagtap.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrnlbrhx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2osjnuwyu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhauktri.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2byyybozf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mkaybmxe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2glcfhxwt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mcqxmzjy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2waxroprx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vkuuhzda.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xnfnzale.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oqyqtzpu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2huvotuqa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xnbvkraw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlruybzi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eldiinog.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jdbakwid.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ctqpqwbn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tzlfedak.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2nlbyomke.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yyrnejvd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ntefyeln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfjtxdun.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fqujeayd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onafkxfs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cnqczrkr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2anylombt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhudexhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lvevutax.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2owwnoeij.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vcqcgefb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2etgamyqe.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrfckjok.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqujyjsq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dpodzbxx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kmnxfjhv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2otkuhbhw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkusxfua.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcfaarko.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqrjapd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2djwuvqlt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gbguwvdq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbyazjpp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2irbzhkkc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2edbbjwbe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tpgmtdou.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qcqyheco.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2imwpoemp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wgejftwg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fshhnntd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2txplqwlp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ipfbbjyz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqxvdtwg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2expdmkqs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zpjfyhko.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qhxvywev.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ezwyrgmn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nyetupfm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wktvgaoz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lozskopt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bnofxzvp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rxgbjyfb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wjdllzgm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wjgewbly.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ailgbthv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyunwdyf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sxmsmieb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pvwknjtm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipyizoqc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oraxcifq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rjlzdgue.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpvluhla.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfzythzg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebmocbtl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dndfibvk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hlwjgngq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfvqgdsq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abyttwsk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ztfmszax.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cdynbiam.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvgyfeb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2actbtuxx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mokubwjj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kkhlgyqa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2cqikoxje.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mrdztywi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2heynwnec.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xdizfrja.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2usdhqxjw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sbpqjtix.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ojnmetrr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gckmumgp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xueyraof.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kgzvybil.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fssallqm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lghwtucv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2swidlgwl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vekbpohy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pivdnits.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lhtckkmu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iptyscst.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rgnrrdce.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2npwzymlj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2estzqwcl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulmwtqei.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tjsygfij.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tdlgtzzq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nffztehx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrgzined.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkthflek.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tisrreob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lvcxscno.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfqqfcil.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ayxadvcl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxlpqtuw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ioojhnvt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mphdvjsb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkiccsai.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovfjvzsr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgtfkmdp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hvirrvio.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wxzaircw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwuoxrjx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2flbjcizt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rdhhhvnq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2aposbvcn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2byvvkcbm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ojmpbfyn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tvkozfwc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2updfnxpa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lznfmzkf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tizcqpeg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ohofieqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnmtukkt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xlefiulc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqppdnva.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2enkufcnl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rtlvikda.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2weziucrb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcvssmgc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rgvyukrc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bibobjor.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vsjwsjff.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rbfhblxy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kmmlywqf.html


<!-- 参考信息 -->