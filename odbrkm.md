代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtfomkkrjz.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtnbrkejxt.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangtech.top/gtxgomltlh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gogol.net.cn/gtegqwwyyu.html

PHP:  strpos($s, "x");
来源：http://hz.gogol.net.cn/gtujtxljzz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj202588.top/gtjxwbwahd.html

TS:   s.indexOf("x")
来源：http://hz.jiagoushi.top/gtoueyjues.html

Java: s.indexOf("x")
来源：http://hz.xylfe.cn/gtsbpotrmi.html

Go:   strings.Index(s, "x")
来源：http://hz.zhiwuduotai.top/gtmgrvopjn.html

Ruby: s.index("x")
来源：http://hz.yanxiufei.cn/gtaefmxyfn.html

C#:   s.IndexOf("x")
来源：http://hz.chenlongwang.top/gtwlmhdyvf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuetiantiany.cn/gtkwhlpqyr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xylfe.cn/gtxoryxtox.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtbqzsknhb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtedlxngyi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydjk.org.cn/gtdzdcukyo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yangfankeji.com/gtrwdbomwq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhoulong.xyz/gtawiwfbpx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xingfuxueyuan.xyz/gtjjmuclyf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenzaomai.com/gtdvcdlsut.html

[E06] 替换子串
来源：http://hz.xylfe.cn/gthjahfstk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shzxlz.cn/gtyyllunro.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.svipenyu.cn/gtjpatvupg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtuqllnblu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtziwdsmjw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtvbcxggkh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gtufuzjzwh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtbpqhegfv.html

C#:   s.Replace("a", "b")
来源：http://hz.sufxvd.cn/gtnhjfjdbx.html

[E07] 按分隔符拆分
来源：http://hz.yj20258888.top/gtsmcgdyki.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ppjwa.cn/gtmmyfrznz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.0kj1m.cn/gtaybnzcpf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuanzx.com/gtkjvpousf.html

TS:   s.split(",")
来源：http://hz.zhaomingkeji.xyz/gtzftiwexv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinyuanbaomall.cn/gtomvbsfil.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtwcvafvxr.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangtech.top/gtlczjnqsz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtyxsubbgm.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtalcxfaqh.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gtnjtzitwi.html

PHP:  implode(",", $items);
来源：http://hz.xinyue.icu/gtamvdhica.html

JS:   items.join(",")
来源：http://hz.yongpay.top/gtaplseuoj.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtghaqelce.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gttjbwgvac.html

Go:   strings.Join(items, ",")
来源：http://hz.fzhhl.top/gtwocuvsht.html

Ruby: items.join(",")
来源：http://hz.hnqzz.top/gtsmudckfh.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gteuqwpurl.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtspcopjsm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinyuanbaomall.cn/gtwcdziypb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gotoacloud.top/gtfgmfuhli.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtqreugcpj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtclitbtqg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtqgbziuwj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guowangkeji.top/gttryvcvkh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtwugsfcdl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daria6918.cn/gtuuwjlwfz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtabelqyzr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dianchejie.cn/gtfyajkwov.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.andypj.xyz/gtijiyvteh.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtuvdajivd.html

TS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtmhqucmrw.html

Java: String.format("%03d", 7)
来源：http://hz.ehwqpu.com/gtwftzpzop.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gtriflnaho.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fengsongda.top/gtapplfodz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtjwkmiipn.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtqjvwkxfw.html

Py:   s[::-1]
来源：http://hz.cheryme.top/gtmcqcisnr.html

PHP:  strrev($s);
来源：http://hz.pengpengdd.cyou/gticlzrqlv.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtdvvbjnnd.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtljyshhja.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xinyue.icu/gtqdkuzrfc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gtabhhtowf.html

Ruby: s.reverse
来源：http://hz.yonumen.top/gtuzznndas.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtogbdffoo.html

[E12] 统计某字符出现次数
来源：http://hz.feifeiyinyue.top/gtgzsoiwaq.html

Py:   s.count("a")
来源：http://hz.pengpengdd.cyou/gtjtnzgcpu.html

PHP:  substr_count($s, "a");
来源：http://hz.hysaishi.cn/gtvlodswca.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtfplfbaib.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtvtofdnhw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.smart0.xyz/gtiadulzrq.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gttupcjypx.html

Ruby: s.count("a")
来源：http://hz.haohaochexian.top/gtdagsqsez.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangshuangyany.cn/gtbefmcsio.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtzyhjlalv.html

Py:   for ch in s: print(ch)
来源：http://hz.ybcxt.top/gtluqoxcwm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.havefunace.top/gtaxdslrac.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtyemjbpys.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gtejcsjwiv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtbuegyiqk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhiwuduotai.top/gtlwkcigse.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zdqjudy.top/gtgmjqmewo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gzhubu.top/gtgztfgele.html

[E14] URL 编码与 Base64
来源：http://hz.sweek.top/gtqkydkjbw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sufxvd.cn/gtvnnxrojq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nwbrower.top/gtuuqgnhmu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ybcxt.top/gtoypbdsdx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sysykeji.top/gtmuzhmimr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.kuanghao11.cn/gtqxpwhozz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gtbyolcffb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtxctkknwe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gzhubu.top/gtddceygfu.html

[E15] HTML 转义 / 反转义
来源：http://hz.jqgfzy.top/gtkrqammhy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenzaomai.com/gtqzumayxb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhoulong.xyz/gtpweoiwle.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtkjskmidj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhiwuduotai.top/gtabvcwcqa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.andypj.xyz/gtddefuvjy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tianlin.xyz/gtcczsrqdp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jlsjyb.cn/gtvbemxvfi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtjlypeioi.html

[E16] 数字千分位
来源：http://hz.zycfv.cn/gtvgnlzrvy.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtdltaehqg.html

PHP:  number_format(1234567);
来源：http://hz.xinyue.icu/gteyuryqft.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gthykkjsfr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtdjjlhpac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aibaodan.cn/gtrpmhiovk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtxpxgxoxs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.bjfxy.top/gtkdwqtmrl.html

C#:   1234567.ToString("N0")
来源：http://hz.jianghu66.top/gtvbldeint.html

[E17] 首字母大写
来源：http://hz.9152youxi.cn/gtikigqsqo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fzhhl.top/gtzxnjcnzm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuetiantiany.cn/gtqicxrdwt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangdashe.top/gtilgempin.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtgoaelggo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhongyouzk.top/gtwbcfmwle.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtkxqccsgs.html

Ruby: s.capitalize
来源：http://hz.zycfv.cn/gtjuhgweik.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.9152youxi.cn/gtfxgofdvv.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtyptjxsfm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtaryugjcl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gtmhuyfflj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtesdmipad.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtoqsuujub.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yangfankeji.com/gtxgnhzzyk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtrpumfnzn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtpadgifxh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgufenzy.top/gtuzmmwfzx.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtkvswgils.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gtcodlktpc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgfzy.top/gterlxukni.html

JS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtjmbqxhhi.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtuxrpkydv.html

Java: s.lines().toList()
来源：http://hz.zhongyouzk.top/gtecvbbrtx.html

Go:   strings.Split(s, "\n")
来源：http://hz.vqdsnc.cn/gtdeegxrkb.html

Ruby: s.lines
来源：http://hz.yuanzhike.top/gtbbgceihn.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtdzgakogx.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtyfpcousw.html

Py:   if not s:
来源：http://hz.zdqjudy.top/gtecvdyssk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nwbrower.top/gtdgsxehmg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtwhwjfxak.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gthwokctfh.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gtcfenbzsf.html

Go:   if s == "" {}
来源：http://hz.ywan-chungtsiang.top/gtwmmkqohc.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtxlamurey.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xingfuxueyuan.xyz/gtdmsxliba.html

[E21] 超长截断加省略号
来源：http://hz.aibaodan.cn/gtskxjoqum.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtxkyltzxl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gteplccrrj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtbjmmszox.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtcansbnww.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtuoxtvpdt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ehwqpu.com/gtykglqskn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gthciersle.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zycfv.cn/gtwoenxeeo.html

[E22] 字节长度与字符长度
来源：http://hz.jiagoushi.top/gtvzfyzsuh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gtgygimezt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gthnblpket.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtpyzsoufy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtvuhrqisl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zycfv.cn/gtcfnofcms.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxuanxn.top/gtqcokqxul.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgufenzy.top/gteyzgmvml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtwjplnbzz.html

================================================================================
来源：http://hz.chenlongwang.top/gtghoglcdt.html

F. 文件与目录
来源：http://hz.bjfxy.top/gtvraufowu.html

================================================================================
来源：http://hz.birdmap.top/gtksyzefrb.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtjsufzphs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj202588.top/gtydpmwlfs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinghuilouyu.cn/gtemryergk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtmsvtnjfo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtfpfktnkf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtmauualvd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.0kj1m.cn/gtapmorfnn.html

Ruby: File.read("a.txt")
来源：http://hz.c1oappe.top/gtabeektzi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.feifeiyinyue.top/gtxevdwlzf.html

[F02] 逐行读取文件
来源：http://hz.shuidangran.top/gttadmamac.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhiwuduotai.top/gtngiyzdng.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtncvtaotw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtoujpkbaw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtfejrvuve.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtwuptqkoo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtxlravzbp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cdnleiting.top/gtwnxdpsfr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gtphatlcrl.html

[F03] 写入文件（覆盖）
来源：http://hz.zycfv.cn/gtcgjnpdkz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gzhubu.top/gtpdbztsqt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtiiwmvbud.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gthrnmdbzq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtdzmdeznp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangshuangyany.cn/gtdrvobbdg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gtwgoitzvw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhaomingkeji.xyz/gtyhbogiyb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuxming.cn/gtchhudwql.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtycdqhvoz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gtdkmbtfzr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtinrocsdt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtoikugruz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtpyvsjoav.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gtqnwlxhks.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258888.top/gtddlxfqif.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtnkiskdgz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgufenzy.top/gtasgkutgg.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gtllzuxtwv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtteqanzap.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gttuvphocq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtqzlysvjk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtpxzvhgii.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtkgdwmsbp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jlsjyb.cn/gtaxyjjlle.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gtllmcymkx.html

C#:   File.Exists("a.txt")
来源：http://hz.redwolf501.top/gtkowuuvtj.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtyttjybru.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtwrspujam.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gtwmrynkkn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtccyyzzke.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtsqrdftba.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtaadxlkjm.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtombgitlm.html

Ruby: File.delete("a.txt")
来源：http://hz.xinyue.icu/gtooqmlhfp.html

C#:   File.Delete("a.txt");
来源：http://hz.ybcxt.top/gthddathsp.html

[F07] 创建目录（含多级）
来源：http://hz.havefunace.top/gtcbdgigmq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xinyue.icu/gtqmsiwmta.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtxaosbyig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtwcwjpecy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtazuvsbxt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fzhhl.top/gtzwcgfxdy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtaugecwqe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sweek.top/gtmgxaqwlo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shuidangran.top/gtxmmynlac.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtjwmlkwvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtmafqlzdw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtzrdvhgdy.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtsxfnvnpo.html

TS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gthxgzlyfe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtzxhfuief.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ehwqpu.com/gtbeiwgxzy.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtfewdxdxu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hysaishi.cn/gtdzfqffwk.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtsaxqgrxu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gtxoesdynx.html

PHP:  filesize("a.txt");
来源：http://hz.pengpengdd.cyou/gtjumzyipm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtdhaddchw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtqzlfpoje.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gthlydibss.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.smart0.xyz/gtqpbdfibr.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtdmufugvy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtwtfschmx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtgemwheaa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtisirxabf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxinkj.top/gtfkddqnyi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtdjduwdcp.html

TS:   path.extname("a.txt")
来源：http://hz.zhoulong.xyz/gtydbyspbo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtrdbxtplv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmtmmydtx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gthnhlllai.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtvhxhdygc.html

[F11] 复制与移动文件
来源：http://hz.yuanzhike.top/gtunajkidq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtbyerasso.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtmhcrcrfm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtkxdrudqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtussdtucl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.c1oappe.top/gtcwoucmpd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtlrnnnsha.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtmlikpvzv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgfzy.top/gthstgfriq.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gtojhzgheq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dianchejie.cn/gtiycbolkp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtqgvmnebw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtrmkmecll.html

TS:   // 同上
来源：http://hz.xylfe.cn/gtasdpfthq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.andypj.xyz/gtvibqhivy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuanzx.com/gtmvowkdpm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gttoylszks.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigufen.top/gtdtrcstpu.html

================================================================================
来源：http://hz.yj20258888.top/gtgsdgzmxx.html

G. 面向对象
来源：http://hz.jinyuanbaomall.cn/gtozadfvqc.html

================================================================================
来源：http://hz.zhixingplan.top/gteinvjhix.html

[G01] 定义类
来源：http://hz.zhaomingkeji.xyz/gtjwzllnyf.html

Py:   class User: pass
来源：http://hz.cucudq.cn/gtypopixxb.html

PHP:  class User {}
来源：http://hz.xinyue.icu/gtonjryuny.html

JS:   class User {}
来源：http://hz.nwbrower.top/gtgoeveguw.html

TS:   class User { name: string = ""; }
来源：http://hz.daria6918.cn/gtfmcqojhh.html

Java: class User {}
来源：http://hz.tanke756.top/gtwmbkhqrd.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtsumvkpwc.html

Ruby: class User; end
来源：http://hz.ywan-chungtsiang.top/gtutoqnanv.html

C#:   class User {}
来源：http://hz.wangshuangyany.cn/gtzjkeoevo.html

[G02] 构造函数
来源：http://hz.0kj1m.cn/gtukesceyk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gtnmjzrvpr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtzchiqyqz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtxcuxenje.html


<!-- 参考信息 -->