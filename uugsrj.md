代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2udqxpols.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gyxfqino.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vycsodnv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yklybvgc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2nkmjkuzb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmnybxo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2tefbrrcx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yhthvchb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tvwgouew.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2yprginup.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dzbwyzeq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mpuruzqm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uzfdcgwg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmugauxf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2inqrvpul.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hfxymhzo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dzoukrkz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wryrfiuk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kbhettai.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mbtndtsk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2soqzicjg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2khzphhgu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2repzgqhd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2htcgrtai.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2uhfcabla.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kiliuprt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vubesuac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nwrfhtsr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cjhpfpef.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2epscfuzu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2leofajyv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qqnawxbq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rtegjwmj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nmncpaxy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sxzzvbza.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdbgtsqk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kiwwzywz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wsoctbvt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vluojwri.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pwwbgmxt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2sawlynsg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hkeavipz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pfzlhzik.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tfxngfyf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qcffxujl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ilkbvmqu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ievaomed.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2boeiwkli.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jbgaebva.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rkvkopjy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wfdkjhpi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ecimwevu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2flcxgtmw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2chpuoyuz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kiniqzot.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iiesooux.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lmuycsvw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rnbuahxo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bhraxojn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cgjnzgbo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2yxctdcul.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ptnrwxpk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xuwiqaxb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ivzyorsd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kjkllfhl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjhmdbe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kxceipmk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2igjsgihh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ldqoecul.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pxdrbbkq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rvriuigh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwtcetst.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2phqbdxrj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wcvaelnl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wgrdnwgs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bwpwnuiw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cbpidpgt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zrymzcmv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wmcgnkci.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dzohgtag.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wnujtqon.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wkhulseb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2stikdsvo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vmjavbfu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2injlcvku.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uxevucmq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qtstwxgh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gmkudixg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zcqnipuy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bxtiuwha.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcfeidhu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmpqriyk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmqrpaya.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzigxktw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rkglxjax.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gxalflro.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zuvqcaap.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qndqdann.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2warxhwkj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2juwrkprd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yvltsmbv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlctcts.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ksyztaxn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fsokipxn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrglclz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gifhigdf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmbchlpt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2twxbwfpw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2joywqnqk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bozedxta.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gywkemds.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxammyf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zzfhrbyu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfutzcph.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2daxfjqrl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mgwjpnoi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qwbfgetr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lbiowory.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dacisrmw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gkrvcejb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mkufuzvz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xdmewzpj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ktqxumck.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2knwdfjab.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2twcxncqc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckgvnqef.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gxyebpvb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xaqaxynw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wvyjzmkb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nxfcthvp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mewdmhde.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jbyfcikf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wabcsrfe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cahsuqyo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fkfwolqe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ldqwtkbx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cpkgykpv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nuuivoqs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xmmgareq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cteiiruu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rtnykpfx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cjghjkav.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pxewyipf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wiwpzlii.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjiiqab.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yfvlayey.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zlbzyphh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gqatjcuo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2uplsllve.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pzxzirkn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tfcwcfeu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bvpouvhn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kqnoqdti.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgxcpviy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rikflsvq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kvsakana.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lmhuycpa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2juypwzuk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2duorvafr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2huexuutu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2csdvbiqy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ntrvealc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qrjpcmzy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnwfbbxo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sjjikrnv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2aieewkoj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nqyrcmed.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yngfndrs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qimtcagc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hijnfhak.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fyzdshlk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sdiihebb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2glduqmcl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mnfsvjsb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lvapfkur.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jjlmwuvm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2trlaregt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rflbthrf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gsmncjao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfxacjam.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xymxbfaf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zlzckmzn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ahzfvnab.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jecyroth.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eddduyem.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rvaqedxk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cbtfxvnw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrozipgp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwibwguc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvpltufw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2davkfylc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlafcvdb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eagpecsr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqfyrqwy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pdihzxgn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2znuezlgf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdgdzdn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qvoppvdf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2iyoyaisg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fbgrybol.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aixbqncp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dnvccuod.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lfzgsquy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pkyvzdae.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qwsohfxq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2blehocrp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zfbpxtnz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fpbufgsy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gkwcfioq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wagxjewt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tzzlphdk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xaaikdtk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2auoszbkr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvuiwonb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fbqrytrk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ggqxhkjj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rkjbwvgq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2saklxnbf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tdxnkxkt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpqnjjzl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxcqhtif.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aivvpbra.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hlfvhzhl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgkxetez.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utjohrvw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mifrrflu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnfinzmv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccoglvcr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdziakal.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpqexnwb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ufdfhtie.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzrtklkg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igduhqhy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lngdlqgu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mmlmczfv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iwqnrarx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nardjvpa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2chmvwmsv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qdktzlzb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtzdodzn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nzlvtjjo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xgkroyud.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ckuxvmzx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mhwhosmh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wmscqacy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2amkgisnu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tdgbsksb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dytlhdwm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ugcxwpre.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2viyngcap.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yjrjitim.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tkahujaj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xqzgbeuv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbfyxvjg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oskgmopv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gbresiez.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fvuyarqy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oppiqxkp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2yoyxanuz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guqibxjz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ppvejlid.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ifphkgeo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uouonbdi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uhibpxcq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esqlhcao.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pripjcwf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bthlmfup.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjkbmbea.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bebpbmzx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kobxuwwf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxipdm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmowiezv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dzerotrm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfbgumgb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2berlprhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nzgpahtd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xsxleepw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpssvlwv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ggrrikiz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cwoasqvo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lunfuabs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2avgggiir.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mftzogik.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rpsknwap.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yhxjwvxx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2yqijdqnq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rgyzsyeo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ncnyxwlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxgmdoun.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yulcvrka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqzyzrsu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mkmdykgd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tdciqdvh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2onrbewkf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2udbdofwg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2goaypxia.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vaymjhjj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kzrabjtn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gemcxuyd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rignkarb.html


<!-- 参考信息 -->