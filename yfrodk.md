代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinqigfzy.top/gtlzezvddp.html

[E03] 截取子串
来源：http://hz.nwbrower.top/gtoicbaaed.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhaomingkeji.xyz/gtqcjbzghv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtdpfcagcg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtnsbrvlea.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gthqbszxmv.html

Java: s.substring(1, 4)
来源：http://hz.yonumen.top/gtxbcidvsz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hfpthk.cn/gtnhmfsypa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hammf.cn/gtunftqxqw.html

C#:   s.Substring(1, 3)
来源：http://hz.smart0.xyz/gtfsocqxjs.html

[E04] 查找子串位置
来源：http://hz.shuidangran.top/gtudavhzpk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ehwqpu.com/gtuihjasqm.html

PHP:  strpos($s, "x");
来源：http://hz.jianghu66.top/gtkviqgaks.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhoulong.xyz/gtswtupfof.html

TS:   s.indexOf("x")
来源：http://hz.yj202588.top/gtdfdbmkdy.html

Java: s.indexOf("x")
来源：http://hz.birdmap.top/gtyoekgbkl.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258888.top/gtobypvacq.html

Ruby: s.index("x")
来源：http://hz.nanxinkj.top/gtbiqqvmgw.html

C#:   s.IndexOf("x")
来源：http://hz.zdqjudy.top/gtfdpclgqg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigfzy.top/gtcbznqyfe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gthvovvypy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtatsmsfsn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgfzy.top/gtdtllitsj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtkiqnmtew.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtayqhusvb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xylfe.cn/gtbwzndxla.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cdnleiting.top/gtogzvzjjr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pengpengdd.cyou/gtotscyqcn.html

[E06] 替换子串
来源：http://hz.ywan-chungtsiang.top/gtwvjpevty.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtzuhmlbna.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.wangshuangyany.cn/gtiwiixqyr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtegsmomyt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtjqbvkwrj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtphasfwue.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yvedp.cn/gttnhbilgi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.wangshuangyany.cn/gtrrtnzbpq.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtkcwzhprp.html

[E07] 按分隔符拆分
来源：http://hz.tian-w.cn/gtixujpqov.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cqqwz.cn/gtgbzkihzs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shuidangran.top/gtegziknra.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenjidiqi.icu/gtzidkovls.html

TS:   s.split(",")
来源：http://hz.shangyingyoupin.top/gthfcazuzi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.birdmap.top/gtdntxopxh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtussfucqb.html

Ruby: s.split(",");  s.split
来源：http://hz.xylfe.cn/gtauhhczdo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xuanzx.com/gttnhfqdwb.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtcwtkossb.html

Py:   ",".join(items)
来源：http://hz.shuidangran.top/gtadlabofi.html

PHP:  implode(",", $items);
来源：http://hz.ppjwa.cn/gtdvkcmukk.html

JS:   items.join(",")
来源：http://hz.wangdashe.top/gtadiwdoha.html

TS:   items.join(",")
来源：http://hz.yongpay.top/gtdpozfqmk.html

Java: String.join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtutekgzzq.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gtwiivjzov.html

Ruby: items.join(",")
来源：http://hz.jinyuanbaomall.cn/gttpxooxil.html

C#:   string.Join(",", items)
来源：http://hz.yonumen.top/gtssrsiudh.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gtafuuwhhm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shangyingyoupin.top/gtfqtlqdur.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aizwys.cn/gtviuybzkt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtrllxykxr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtjwdmdspy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.bjfxy.top/gtiyvbrutu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtwlxecrgt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yonumen.top/gttnkcqxrj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sysykeji.top/gtjjtieefv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cqqwz.cn/gtthvsbgam.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sxryk.cn/gtmwjnqpxg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtbwksqpvc.html

JS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtmpppdota.html

TS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtwyfkwoma.html

Java: String.format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtthttgrpt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnxiangtu.top/gthpagafdf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuxming.cn/gtmsrorszx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhiwuduotai.top/gtlmqrwkmg.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtlekdemqb.html

Py:   s[::-1]
来源：http://hz.ehwqpu.com/gtuaxedvlg.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtgsrwuwtu.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtmjhmmyfb.html

TS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtfkrcbjln.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guannengcc.top/gtnwnmyvzf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pycfn.com/gtpbjsorre.html

Ruby: s.reverse
来源：http://hz.9152youxi.cn/gttnegctka.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtxnspnxpg.html

[E12] 统计某字符出现次数
来源：http://hz.birdmap.top/gtypyagaun.html

Py:   s.count("a")
来源：http://hz.yvedp.cn/gttknladkj.html

PHP:  substr_count($s, "a");
来源：http://hz.zhijiandao.cn/gtrquvpiuv.html

JS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtnnnwxtkm.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtdjdiyzge.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuanzhike.top/gttxmbjsej.html

Go:   strings.Count(s, "a")
来源：http://hz.dashuyun.cn/gtngzmzykg.html

Ruby: s.count("a")
来源：http://hz.yangfankeji.com/gtfojzyrlt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fengsongda.top/gtillqbuxq.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtldutyexi.html

Py:   for ch in s: print(ch)
来源：http://hz.chenzaomai.com/gteevlwqhl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gtjxlcphyg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtdphuyvyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtwfeqgqhu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jqgufenzy.top/gtcjooyxmj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtfnmmsaom.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ybcxt.top/gtoowafptw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtlmdzgyan.html

[E14] URL 编码与 Base64
来源：http://hz.xinyue.icu/gtvlghiliw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.kuanghao11.cn/gtctgtipcp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtvibxagdh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.redwolf501.top/gtfmovkfqw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ppjwa.cn/gtbzckfkgw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhaomingkeji.xyz/gtvsriulha.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ehwqpu.com/gtutauqfln.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenlongwang.top/gtgdsqihom.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.redwolf501.top/gtqmedrafi.html

[E15] HTML 转义 / 反转义
来源：http://hz.hywenlv.cn/gtbtxfiblm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gogol.net.cn/gtqcllbgym.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pengpengdd.cyou/gtttojmokx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daxiang520.top/gtxmkicdyd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.quarkkingdee.top/gtwlnmdabn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xylfe.cn/gthtoykdif.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinyuanbaomall.cn/gtmeeceidd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtshjcxbdg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj202588.top/gtrnrtretf.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtuwdxqtah.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gttwigxrug.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtbtxtrwfz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtlqxfcgfv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtqievessg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtjlrnwfpn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxinkj.top/gtzcjengib.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtffmslmql.html

C#:   1234567.ToString("N0")
来源：http://hz.fzhhl.top/gtmtpciqxj.html

[E17] 首字母大写
来源：http://hz.nwbrower.top/gtizaybyor.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangdashe.top/gtyjwemvuq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.kuanghao11.cn/gtstgshmxs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jlsjyb.cn/gtcevsfhwu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtrzfjwdzb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtahiggqzz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hfpthk.cn/gtibworfzc.html

Ruby: s.capitalize
来源：http://hz.feifeiyinyue.top/gtjsltlajr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.iojbl.cn/gtlfrtjphd.html

[E18] 模板占位符替换
来源：http://hz.zhongyouzk.top/gtvrhwyvhy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtmpyjndwb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shzxlz.cn/gteenigjot.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gtuewimimw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gthqxoimid.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sysykeji.top/gtywjzehcf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hongshengwenyu.top/gtdycfooxs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtqbjjmjqn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.birdmap.top/gtfuokzkys.html

[E19] 多行文本按行拆分
来源：http://hz.meibo888.top/gtcxvgcipb.html

Py:   s.splitlines()
来源：http://hz.chenjidiqi.icu/gthzhfmhqe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dashuyun.cn/gtrhzucsmg.html

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtxerwkejs.html

TS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtwnwqqjgs.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtudhsfjrt.html

Go:   strings.Split(s, "\n")
来源：http://hz.sweek.top/gtfzdrrjuc.html

Ruby: s.lines
来源：http://hz.nanxinkj.top/gtzxoxxabv.html

C#:   s.Split('\n')
来源：http://hz.guannengcc.top/gtccbyqoqp.html

[E20] 判断字符串是否为空
来源：http://hz.shangyingyoupin.top/gtaclloiac.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtljjdavxi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.bjfxy.top/gtppjldsbs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtckpbibuh.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtwimoepez.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gtpqocyler.html

Go:   if s == "" {}
来源：http://hz.sxryk.cn/gtcbskrwdw.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtyiaqyyrk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenjidiqi.icu/gtyliernlk.html

[E21] 超长截断加省略号
来源：http://hz.nanxinkj.top/gtrmhbyfvy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgufenzy.top/gtecmmfgmv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtodfmnbrk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtxjagblxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gthkhvfrok.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtveuwggre.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cashguo.top/gtpikbvjrw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daria6918.cn/gtylbdojls.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sxryk.cn/gtwbrautsi.html

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtpuzjqedc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtkxmmyynm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtpijxpwse.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtbzkpvdar.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtfkhnnxpd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.haohaochexian.top/gtoznkrksp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.smart0.xyz/gthnnsmjze.html

Ruby: s.bytesize;  s.length
来源：http://hz.jianghu66.top/gtdytgjomg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shuidangran.top/gtoxxnnivx.html

================================================================================
来源：http://hz.daria6918.cn/gtcgftqmaw.html

F. 文件与目录
来源：http://hz.jinyuanbaomall.cn/gtqtskxvaf.html

================================================================================
来源：http://hz.birdmap.top/gtzhitirlh.html

[F01] 读取整个文件
来源：http://hz.dashuyun.cn/gthdshkhhd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtbtkcjetv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtnwtetisq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtzhggqfck.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daria6918.cn/gtjasrzfqp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtgczyvquq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtdmgxaiev.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtuoujotso.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.meibo888.top/gttfdzppua.html

[F02] 逐行读取文件
来源：http://hz.yuxming.cn/gtvnvpjeex.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtexuryhfo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.feifeiyinyue.top/gtuuaarlkc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtnexhwfml.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtoeaxjdwk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtvkaanydk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aizwys.cn/gtahnxotxt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cdnleiting.top/gthatichik.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.bjfxy.top/gtuyrkuiaa.html

[F03] 写入文件（覆盖）
来源：http://hz.xuanzx.com/gtwqmflyjh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxinkj.top/gtslbpitlr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtlclnslcd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtfbgnopwr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtwtnliomj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtsoxnpegk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhengqikj.top/gtzjfgexdc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhongyouzk.top/gtqhcefxuh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtqosjdijm.html

[F04] 追加写入文件
来源：http://hz.316326.xyz/gtznzhewcj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shzxlz.cn/gtyozfroln.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtsrswaeci.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtiemujfdd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gteylwzamh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxinkj.top/gtaaoikcbb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gotoacloud.top/gtaqqljlgd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenlongwang.top/gtspsnkflc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnxiangtu.top/gtyrjzlpau.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gtsgszuhqr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.meibo888.top/gtmianqvmx.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtelmfhxil.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtaqadefja.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtxgjzrcvm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gturifiuzl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtishvxvqv.html

Ruby: File.exist?("a.txt")
来源：http://hz.jyoumei.cn/gtijieiygz.html

C#:   File.Exists("a.txt")
来源：http://hz.nwbrower.top/gtriwaggzq.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtckqwsdtm.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gtxgkuplrd.html

PHP:  unlink("a.txt");
来源：http://hz.tanke756.top/gtvvffibeb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtcxldqthv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtwulmcwnn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtdfpgskpg.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtugopacsw.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtohzzzbqv.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtvrllcref.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtmfgqwfxg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtyqvhzjmm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtivoumhyx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtezxcjbhf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtgfxhwtbp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtqrujoojx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gtffacferq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.birdmap.top/gtdrrmwtvr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhoulong.xyz/gtzdpcwsic.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtwqdgzipq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ybcxt.top/gttthcygrg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.quarkkingdee.top/gtcxxlvjxt.html

JS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gttrimwisa.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtfyakpxma.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtnlljyrfu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aibaodan.cn/gthggcnhfa.html

Ruby: Dir.children("dir")
来源：http://hz.sxryk.cn/gtlfcaopqz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.bjfxy.top/gtlgbmeiic.html

[F09] 获取文件大小
来源：http://hz.yj202588.top/gtvsrwfbni.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gtigzixzpb.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtbgzxgmza.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtlggdrxcj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtwgdyrqzl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtewnxoynf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xinyue.icu/gthgwsbulo.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtnnjjrqgo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhaomingkeji.xyz/gtjvypmgzk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gttahwpkqd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtznsgvpmm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hfpthk.cn/gtympwfjoa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtbovorygj.html

TS:   path.extname("a.txt")
来源：http://hz.yuanzhike.top/gtlbahnvxt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gtkyhsxpja.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdixyopun.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtzfhmsyez.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtrqzzfvgl.html

[F11] 复制与移动文件
来源：http://hz.dianchejie.cn/gtopfoacsk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtujndmlbd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yonumen.top/gtfptecegu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtsjzdjkja.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtcefqzpnp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtikduiqbv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtljhiguwm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtqkdgvwia.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxinkj.top/gtiyzlaphu.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtafzwdclh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtzyjoaubx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtpgwnjzfq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ywan-chungtsiang.top/gtbgpwdknh.html

TS:   // 同上
来源：http://hz.cqqwz.cn/gtzwxddbvc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gotoacloud.top/gtovultwba.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.feifeiyinyue.top/gtkejzfnuc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtspbxaxtw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhengqikj.top/gtbsgblrsq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtboufbtlu.html

G. 面向对象
来源：http://hz.52xcode.cn/gtchnvbcmr.html

================================================================================
来源：http://hz.hywenlv.cn/gtofnrgwyf.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtsyncarnd.html

Py:   class User: pass
来源：http://hz.ybcxt.top/gtbqjrmglr.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtwgtoxzhp.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtiqqaguxy.html

TS:   class User { name: string = ""; }
来源：http://hz.hnxiangtu.top/gtsqptgkor.html


<!-- 参考信息 -->