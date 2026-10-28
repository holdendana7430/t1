代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dashuyun.cn/gtdcmasvmh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydjk.org.cn/gttnjpsbor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtmaodozhj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gotoacloud.top/gtozkzjlga.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtgeblajqp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sxryk.cn/gtambraags.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.c1oappe.top/gtykoesyiw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtnnvcglvb.html

[E06] 替换子串
来源：http://hz.jinghuilouyu.cn/gtqkkafmmi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zycfv.cn/gtggdrkjpb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhongyouzk.top/gthdfrumat.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtzitdubct.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gticodjleh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtubluyevk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenzaomai.com/gtdgrrxkge.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuetiantiany.cn/gtzbvfgxiu.html

C#:   s.Replace("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtyvdtoslj.html

[E07] 按分隔符拆分
来源：http://hz.ydjk.org.cn/gtxipuizqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hfpthk.cn/gtwgkchtec.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtmfwugjab.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jyoumei.cn/gtbcnhmygy.html

TS:   s.split(",")
来源：http://hz.ydzc1.top/gtiwkyhykr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.haohaochexian.top/gtzxchkxad.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtewhwvldw.html

Ruby: s.split(",");  s.split
来源：http://hz.yueranfly.top/gtqccblfbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.9152youxi.cn/gtfatesgke.html

[E08] 数组按分隔符合并
来源：http://hz.tian-w.cn/gtatemoeug.html

Py:   ",".join(items)
来源：http://hz.xuetiantiany.cn/gtjrezvhfq.html

PHP:  implode(",", $items);
来源：http://hz.jqgfzy.top/gtxdaetgas.html

JS:   items.join(",")
来源：http://hz.hfpthk.cn/gtgkpvxwfd.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtujuovgtl.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtkyfcbmac.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtlglyuucb.html

Ruby: items.join(",")
来源：http://hz.jinqigufen.top/gtxtqgxonk.html

C#:   string.Join(",", items)
来源：http://hz.wangdashe.top/gtlfynqnec.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gtljdshbpu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtbugbvkhz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.c1oappe.top/gtzhotqcfb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtaqjswhad.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtnoskjvoh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yanxiufei.cn/gtuckfjtio.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.birdmap.top/gtfrypchxg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cdnleiting.top/gtlaubwrbg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuetiantiany.cn/gtpwflsydu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtyuwlotpp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtwqkzgpug.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fengsongda.top/gtnszsbuxo.html

JS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtsahnmrbb.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtxdsrmqpf.html

Java: String.format("%03d", 7)
来源：http://hz.xinyue.icu/gtkuoiical.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guannengcc.top/gtdnyjuynb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ehwqpu.com/gtszjcudud.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gaohongyu789.top/gtwpshzikk.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gteweomeqv.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gthxetghng.html

PHP:  strrev($s);
来源：http://hz.jqgufenzy.top/gtapjytlrp.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtpltubyeo.html

TS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtxeyoabyt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnxiangtu.top/gtzffddtmt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gthfyypqro.html

Ruby: s.reverse
来源：http://hz.316326.xyz/gtjqlbqexi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtoluhmzxh.html

[E12] 统计某字符出现次数
来源：http://hz.aibaodan.cn/gtsptwedfm.html

Py:   s.count("a")
来源：http://hz.daria6918.cn/gtawwoydoa.html

PHP:  substr_count($s, "a");
来源：http://hz.jianghu66.top/gtroeaqrzj.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtsmoscfic.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtnwjhxodi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cucudq.cn/gtytsxopwp.html

Go:   strings.Count(s, "a")
来源：http://hz.ydjk.org.cn/gtioyxrgrn.html

Ruby: s.count("a")
来源：http://hz.havefunace.top/gtaixbxoxf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dianchejie.cn/gtzrsxecxa.html

[E13] 逐字符遍历
来源：http://hz.c1oappe.top/gthnzwonnc.html

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gtiummepub.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtppoacnhn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gttkicswcs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtssmhywnq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hysaishi.cn/gtkoxtbaqd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pycfn.com/gtotllrcov.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenlongwang.top/gtceevonmp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.vqdsnc.cn/gtzspbdytb.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gtzllldbiu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuxming.cn/gthqiiezhd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj202588.top/gtmlkllxga.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.52xcode.cn/gtbqmairii.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtpvjiawxn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuetiantiany.cn/gtixxqdrwb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ywan-chungtsiang.top/gtpjjlmmrb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtzegbglsm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtqtcrgkhe.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtwygixncv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.haohaochexian.top/gtgzyqdvrg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydzc1.top/gtvzsmwyia.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.birdmap.top/gtyhqkriwm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cucudq.cn/gtjmxrpqhe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtcefcvfhu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.birdmap.top/gtxajmhrno.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gttwgvcsjm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.quarkkingdee.top/gtpjmrcjuu.html

[E16] 数字千分位
来源：http://hz.9152youxi.cn/gtvaxutnmn.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gthwftniyf.html

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtuyqteedk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtnahhtfhd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtakvnqipn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtcxaqvxke.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangkeji.top/gtfwcbxqfx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydjk.org.cn/gtnovzsaes.html

C#:   1234567.ToString("N0")
来源：http://hz.9152youxi.cn/gtzclrmakd.html

[E17] 首字母大写
来源：http://hz.cqqwz.cn/gtoakwjsqm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtdmfuzdqj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.fengsongda.top/gttwdkpmmd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtnlekjfck.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtvqbrorrl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.meibo888.top/gtwvpibfqd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aizwys.cn/gtrlyiqumc.html

Ruby: s.capitalize
来源：http://hz.kuanghao11.cn/gtetanncwb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daria6918.cn/gtrtikulxl.html

[E18] 模板占位符替换
来源：http://hz.tianlin.xyz/gtbefgoupk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gteovsqthz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtebhakbfg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtkbwwbpwg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtutvrwiot.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtyivdbvtv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cqqwz.cn/gtlpvwuvpu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yonumen.top/gtkmlptirr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtszvaoqql.html

[E19] 多行文本按行拆分
来源：http://hz.sxryk.cn/gtmhckhdga.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtpokqnqnj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gtonrskdop.html

JS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtfarymmtf.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangtech.top/gtlozvrwca.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtkhbhihau.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangshuangyany.cn/gtmcnlfrnn.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gttxliwgqx.html

C#:   s.Split('\n')
来源：http://hz.zdqjudy.top/gtmwgnqcje.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtnhcdhkca.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtvbxmnlzv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.andypj.xyz/gtpnugrvrz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.feifeiyinyue.top/gtzyhyajcl.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtnfycrkdz.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtlhudjytt.html

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gtnvksppec.html

Ruby: if s.empty?
来源：http://hz.iojbl.cn/gtzsniqclp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtgulnbqxy.html

[E21] 超长截断加省略号
来源：http://hz.vqdsnc.cn/gtahxjczpf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtlixofrnk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtiqckfijc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtuijmvckl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtvvfecufs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtqqgvvamx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ivvv.top/gtgzgtvmsf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtdldjwctc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yueranfly.top/gtfosjgehm.html

[E22] 字节长度与字符长度
来源：http://hz.pycfn.com/gttmoiwywx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtoyydstaa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtrgfivqus.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtlzngsdhm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtgxirzmnx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtmxfixxql.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuanzhike.top/gtkbnsnwjx.html

Ruby: s.bytesize;  s.length
来源：http://hz.mhx1999.top/gtyfimoodu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtxfplwzvk.html

================================================================================
来源：http://hz.yuxming.cn/gthydfwlan.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtmmfynoxa.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtrgousdeb.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtqabtsldv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nwbrower.top/gtzgrgxers.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ivvv.top/gtftnwbjqr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gthzlbmoyi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jianghu66.top/gtznfshvxz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtilfzsifl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtvfthvvby.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtehaagocm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tanke756.top/gtjzcpufpb.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtvhlbjsvk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinghuilouyu.cn/gtkffcwrxa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zycfv.cn/gtnfxvxvtp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtwzajkxwn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtqtteoprj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtpwozjtcd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtjzutqbdf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuanzhike.top/gtolgsgjgr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tianlin.xyz/gtgowhlohp.html

[F03] 写入文件（覆盖）
来源：http://hz.redwolf501.top/gtelhydrio.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aibaodan.cn/gtdwsnqzyr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yongpay.top/gtqptsxzzf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtedvbldlv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtouojjwbo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gtbwzmbuiv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gthgtzofza.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gtwpzpywmb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtxxsjfcrc.html

[F04] 追加写入文件
来源：http://hz.sxryk.cn/gtharlnnkk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cqqwz.cn/gtwdhyvgjc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtczphdjvr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtyshilbli.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtuucicmbz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nwbrower.top/gtfzilstez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sysykeji.top/gtmhvhzznu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgufenzy.top/gtwiriorpj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtzumfpxap.html

[F05] 判断文件或目录是否存在
来源：http://hz.jianghu66.top/gtpkwrdupn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gzhubu.top/gtcainmfck.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtqssqgayr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtvafcbtji.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtcjwniahe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtqihqgmaj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yangfankeji.com/gtikcfhvmi.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtnughdxga.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gttihfdkyo.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtxjdtnrff.html

Py:   os.remove("a.txt")
来源：http://hz.zhijiandao.cn/gtxcodisuq.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtgnyxzies.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtbxawhixr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtrpmmdrzq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtegotpzob.html

Go:   os.Remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtlkisakjd.html

Ruby: File.delete("a.txt")
来源：http://hz.hnqzz.top/gtodqmioyh.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gtnhofmjif.html

[F07] 创建目录（含多级）
来源：http://hz.smart0.xyz/gturlunsfd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtissddqyc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hfpthk.cn/gtcoupnlmk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtxglueros.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtlxhznkqa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtpgxraznq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gttyntudnj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtwnrbalgj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gtkqdnvtjw.html

[F08] 遍历目录
来源：http://hz.nanxinkj.top/gtfvszyrdh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cheryme.top/gttzppvgre.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenlongwang.top/gtjsccvxay.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtcymibvrj.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtluzewgol.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtrowhdiza.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.316326.xyz/gtdvkynksb.html

Ruby: Dir.children("dir")
来源：http://hz.daria6918.cn/gttddhklau.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinyuanbaomall.cn/gtchkoiuca.html

[F09] 获取文件大小
来源：http://hz.hysaishi.cn/gteleysarq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtnkvkakfw.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258.top/gtraistlcd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtjtudkqgy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtaqoumszg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtslmfqnwz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gttpqwigkc.html

Ruby: File.size("a.txt")
来源：http://hz.jyoumei.cn/gtmdvyooko.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tian-w.cn/gtwtanikvp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jyoumei.cn/gtaoeciegb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtisgmadoi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhixingplan.top/gtclkyrelt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtizwnxayq.html

TS:   path.extname("a.txt")
来源：http://hz.hnxiangtu.top/gtoghrzdtv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtavcwrtix.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtdbdvuigj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtdywbjtgs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fengsongda.top/gttdrapcyh.html

[F11] 复制与移动文件
来源：http://hz.hfpthk.cn/gtkbeqzoex.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtabarullv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cheryme.top/gtvxsotmlo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtxqvgettv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gthktezrez.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtbvzocfrp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtltugzwft.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtzheailru.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtliucgbju.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtifkxyurr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yueranfly.top/gtadlokcrm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jiagoushi.top/gtzzdonrsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.c1oappe.top/gtjztgmwil.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtgtmiqiyx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtvwqenaqi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtpxmebggp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtbqxvmfez.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gtsdxpuucl.html

================================================================================
来源：http://hz.wangdashe.top/gtnzsuiheu.html

G. 面向对象
来源：http://hz.tianlin.xyz/gtsdorfbso.html

================================================================================
来源：http://hz.cashguo.top/gthgfsazoy.html

[G01] 定义类
来源：http://hz.yj202588.top/gtsjiktfvu.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtmiobtbae.html

PHP:  class User {}
来源：http://hz.sufxvd.cn/gttacocank.html

JS:   class User {}
来源：http://hz.jqgufenzy.top/gtmdkahmvf.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtwcwzeikn.html

Java: class User {}
来源：http://hz.xylfe.cn/gtvvacvjci.html

Go:   type User struct { Name string }
来源：http://hz.xuanzx.com/gtmkdxnyht.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gtzqmcpypg.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtiuwcdevy.html

[G02] 构造函数
来源：http://hz.xziqi.cn/gtlnnytmru.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydjk.org.cn/gttftwzpmz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hysaishi.cn/gtatwrmvso.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gteyibldyw.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtdnetezvx.html

Java: User(String name) { this.name = name; }
来源：http://hz.iojbl.cn/gtrnsczghn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtssbhilzs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cheryme.top/gtupddxspv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zdqjudy.top/gtkvhbtjqx.html

[G03] 实例属性
来源：http://hz.cheryme.top/gtwpvsnaof.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtgdtfmskk.html

PHP:  public string $name = "x";
来源：http://hz.gotoacloud.top/gtcpabyzwx.html

JS:   this.name = "x";
来源：http://hz.hfpthk.cn/gtvnxdidvd.html

TS:   name: string = "x";
来源：http://hz.jlsjyb.cn/gtmakdulxj.html

Java: private String name;
来源：http://hz.pycfn.com/gtpfhxozql.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtyetfvcqq.html


<!-- 参考信息 -->