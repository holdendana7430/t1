代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.sweek.top/gtopwxbgux.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gtiwfuzzhe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxinkj.top/gtopoeplug.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yonumen.top/gtnyqpydgk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.0kj1m.cn/gtvsljonpp.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtybcaegdy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnqzz.top/gtayydpcoo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sufxvd.cn/gtfoqbaegc.html

Ruby: s.split(",");  s.split
来源：http://hz.cdnleiting.top/gtiztwhves.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtwlpckrjf.html

[E08] 数组按分隔符合并
来源：http://hz.xinyue.icu/gtfinislbb.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtrqbxsoud.html

PHP:  implode(",", $items);
来源：http://hz.hammf.cn/gtainebjtv.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gtbplwevqp.html

TS:   items.join(",")
来源：http://hz.iojbl.cn/gtdwkvzgbl.html

Java: String.join(",", items)
来源：http://hz.fzhhl.top/gtqvhhubzj.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigufen.top/gtjnghtqww.html

Ruby: items.join(",")
来源：http://hz.yj20258888.top/gtioczhnqc.html

C#:   string.Join(",", items)
来源：http://hz.yanxiufei.cn/gtqpnpvntn.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtfncraatf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenzaomai.com/gtnkqtixic.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gtbpnocyej.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtzftksghb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtlactpzej.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.bjfxy.top/gtlfkltxsw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuxming.cn/gtlhtwisye.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtyfgtuxji.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.0kj1m.cn/gtlcvqwlfd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxuanxn.top/gtcrvrwpyq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydzc1.top/gtrdzikfpn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pycfn.com/gtfdstsyds.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtnllauotf.html

TS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtohqshtrh.html

Java: String.format("%03d", 7)
来源：http://hz.shzxlz.cn/gtesfguxyu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tian-w.cn/gtpmtdeycw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gtxcggxqps.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangkeji.top/gthnuwspkd.html

[E11] 反转字符串
来源：http://hz.daxiang520.top/gtceulirat.html

Py:   s[::-1]
来源：http://hz.hysaishi.cn/gtbfmbitmw.html

PHP:  strrev($s);
来源：http://hz.316326.xyz/gtrwumgbea.html

JS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtgwidkyvs.html

TS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gttgmrpfgw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtmxjjkzhl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.daria6918.cn/gtngapxdxx.html

Ruby: s.reverse
来源：http://hz.jinqigfzy.top/gtmmbmrdej.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtnfuhfnbc.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258888.top/gtyjwapcps.html

Py:   s.count("a")
来源：http://hz.pengpengdd.cyou/gtncwqfqsc.html

PHP:  substr_count($s, "a");
来源：http://hz.chenjidiqi.icu/gtclybqrfb.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtxgoxpljx.html

TS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtfovyfvqk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sweek.top/gtihetjagg.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtmpnpuamr.html

Ruby: s.count("a")
来源：http://hz.jyoumei.cn/gtgeyewlos.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtbncreula.html

[E13] 逐字符遍历
来源：http://hz.nanxinkj.top/gtfyzqmeim.html

Py:   for ch in s: print(ch)
来源：http://hz.316326.xyz/gtczuksboy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtqcofblyo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cashguo.top/gtdoqvpfzt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtdvdbdwxr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigfzy.top/gtbykbgksp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtgksgryhs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fzhhl.top/gtyptwjlyu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnqzz.top/gtasrjsdev.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtcjunuzsx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sxryk.cn/gtuidvmreu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hysaishi.cn/gthxdetffs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yvedp.cn/gtztldbikn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtzijuwodp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenzaomai.com/gtvhtklezz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtocouqmll.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhaomingkeji.xyz/gthkrfjlmm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yvedp.cn/gtfdacrlei.html

[E15] HTML 转义 / 反转义
来源：http://hz.pycfn.com/gthnoxjsct.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jiagoushi.top/gtuxjwzbvf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gaohongyu789.top/gtdnxmwges.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daxiang520.top/gtmtaelshl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinghuilouyu.cn/gtykqjyzeg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gterbvkqjq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.vqdsnc.cn/gtoilwdblc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jiagoushi.top/gtbxbcffdr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuetiantiany.cn/gtjbbhfpbn.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtyknscqqp.html

Py:   f"{1234567:,}"
来源：http://hz.zhongyouzk.top/gtdaeazsom.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtpczjxhuf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtwuwlvezv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.316326.xyz/gtkxocedon.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtmvhmsfyo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.haohaochexian.top/gtjtkzlcce.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.quarkkingdee.top/gtckuscqco.html

C#:   1234567.ToString("N0")
来源：http://hz.andypj.xyz/gtbfafdxlm.html

[E17] 首字母大写
来源：http://hz.0kj1m.cn/gttvjmukbi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtbyjuaxch.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgfzy.top/gthzysmxot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jlsjyb.cn/gtghfauaaa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtelmidqxk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sxryk.cn/gtjqjnbvbq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.quarkkingdee.top/gthnsynryb.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtzuitgkft.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hysaishi.cn/gtagyjhtbq.html

[E18] 模板占位符替换
来源：http://hz.ehwqpu.com/gtbyvfhdfo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cdnleiting.top/gthnbdavmu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtiysqqxpp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtbqygnocp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtgjwblerm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.quarkkingdee.top/gtirhhcwdk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtmzqqdouh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daria6918.cn/gtjgnohqwf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuanzx.com/gtnoejqaot.html

[E19] 多行文本按行拆分
来源：http://hz.9152youxi.cn/gtocvgfwbg.html

Py:   s.splitlines()
来源：http://hz.jlsjyb.cn/gtdseyvhcy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gtjpsuouei.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtuhfgykip.html

TS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtloahwraq.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gtcrlxnpci.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhijiandao.cn/gtxckllfkm.html

Ruby: s.lines
来源：http://hz.ivvv.top/gtaxlxbhsa.html

C#:   s.Split('\n')
来源：http://hz.yuxming.cn/gthjlvofld.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtgnyflojr.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtxzvzinla.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gttnamaald.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dashuyun.cn/gtrxoqyiay.html

TS:   if (s === "") {}
来源：http://hz.xingfuxueyuan.xyz/gtjrahewnw.html

Java: if (s.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtqaptorfc.html

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gtpbvopnzn.html

Ruby: if s.empty?
来源：http://hz.xylfe.cn/gtfwlagwbb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtrsnmbrqw.html

[E21] 超长截断加省略号
来源：http://hz.gotoacloud.top/gtqykpzcqo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhiwuduotai.top/gtuynreyxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hywenlv.cn/gtsjeqachg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtdlyiupcd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtoctmegcf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtznvogvzp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cucudq.cn/gtbeuklapv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.c1oappe.top/gtixhmcibs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtyqwbvgrw.html

[E22] 字节长度与字符长度
来源：http://hz.pycfn.com/gtoyqpbcul.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gotoacloud.top/gtmywtoxox.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtpkxwbpdt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtzhyzwqrk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtommcrqdw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtkfniliyn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hfpthk.cn/gtjuxocdkp.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhongyouzk.top/gtwajcloam.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenjidiqi.icu/gtropnruju.html

================================================================================
来源：http://hz.snrcjt.cn/gtszdzhrvc.html

F. 文件与目录
来源：http://hz.shanyushiyangkeji.top/gtbdavmwpr.html

================================================================================
来源：http://hz.mhx1999.top/gthcccanvn.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtdtxatcri.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtdxjwtlcp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ppjwa.cn/gtlhzlpguq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhijiandao.cn/gtwnqcjgku.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtotnwhdep.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtekhszmrq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.kuanghao11.cn/gttpkuersp.html

Ruby: File.read("a.txt")
来源：http://hz.meibo888.top/gtqudkzvon.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtqoyupshe.html

[F02] 逐行读取文件
来源：http://hz.cucudq.cn/gtjlpwtqfs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gtfcbnzqmm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gthhjtledp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtnnvfugtm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtprptmvxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtfkizhihh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtzdifvpom.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hammf.cn/gtaikxxhuo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydzc1.top/gtscgfpvzk.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtfinrpbou.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtpleedudl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtxubaegqs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtputmbvoo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtxhpmxgxn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtpuufxavu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtsoxbjqvl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xinyue.icu/gtuzcbmakx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gteqnstcil.html

[F04] 追加写入文件
来源：http://hz.jinqigfzy.top/gtygbabjuo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cheryme.top/gtizwasfbu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hfpthk.cn/gtwctxtdbm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtknefobgw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtatqatpuq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guannengcc.top/gtkedtojyw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gtjilynnmv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gttbgghcoh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtqgbovejk.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinghuilouyu.cn/gtqjapurfg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtylpsvfrd.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtdoajtgep.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtfibyafxy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtypqrjfyy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtpzoeyelh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gtpjviuods.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhiwuduotai.top/gtladxfcka.html

C#:   File.Exists("a.txt")
来源：http://hz.cheryme.top/gthlqqrkwd.html

[F06] 删除文件
来源：http://hz.cucudq.cn/gtstndvvag.html

Py:   os.remove("a.txt")
来源：http://hz.daxiang520.top/gtxnqbdxzc.html

PHP:  unlink("a.txt");
来源：http://hz.zdqjudy.top/gtkmieuqiy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtdfrhfcix.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gthobcfoda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtxzotmbhf.html

Go:   os.Remove("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtnxlljxzk.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangtech.top/gtcszjgxub.html

C#:   File.Delete("a.txt");
来源：http://hz.gogol.net.cn/gtylvrxchy.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtphpfgvxe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtjwyiqjjv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yvedp.cn/gtpnmzgqko.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtjfxwmuuh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtcmkoknvq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtfcdlfgcx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenjidiqi.icu/gtgytyptjs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ivvv.top/gtunggmmhb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yvedp.cn/gtrzclyrns.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gthweibdhc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gtxvlkrwlw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sysykeji.top/gtlvtdmiur.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gthwohsrji.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtkmdirulu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtcfgxzntl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtsxugaaec.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtxdpbklqg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtsaoufoez.html

[F09] 获取文件大小
来源：http://hz.jqgfzy.top/gtkttvumte.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydzc1.top/gtwtwrdtkx.html

PHP:  filesize("a.txt");
来源：http://hz.andypj.xyz/gtseoqkpvg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtkbhssmot.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtemrmdsoz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtjlcdjgzv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtspagydiq.html

Ruby: File.size("a.txt")
来源：http://hz.jlsjyb.cn/gtojzbbqlh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuetiantiany.cn/gtptidunko.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gttcuejmfb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtsbhxasce.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtdtanxeiw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtmhcpmtzf.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtaxazoacg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dashuyun.cn/gttmzbyltz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigfzy.top/gteiomowci.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtqlthlczj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cashguo.top/gtjqyybuqt.html

[F11] 复制与移动文件
来源：http://hz.daxiang520.top/gtnqdowaph.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtucdlpmgj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtwhtpmfti.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtnkgcwrvn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtsbqwlcyx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtpkzvvbuk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtpwqcssow.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtvxyubimt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fengsongda.top/gtrfflduqv.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtetzsmxeu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gzhubu.top/gtyptqorfk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigfzy.top/gtheonycrp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtszasuvgt.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gtsncsnmsv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yonumen.top/gtnromfrkd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guannengcc.top/gteinzcxmg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guannengcc.top/gtdjxqyhqy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtzljucnpa.html

================================================================================
来源：http://hz.jlsjyb.cn/gtuxuxkqil.html

G. 面向对象
来源：http://hz.hammf.cn/gtbdmhdlsi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpjfryhuj.html

[G01] 定义类
来源：http://hz.zhongyouzk.top/gtirgbmbtf.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtxmpoodlg.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtbrzbrynl.html

JS:   class User {}
来源：http://hz.jqgfzy.top/gtqpxlefze.html

TS:   class User { name: string = ""; }
来源：http://hz.sxryk.cn/gtdyhwggxo.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtpiwstjts.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtzydvughz.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gtmigglhhx.html

C#:   class User {}
来源：http://hz.hammf.cn/gtjuqokfnn.html

[G02] 构造函数
来源：http://hz.yongpay.top/gtnepxauio.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtszbhfcft.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.quarkkingdee.top/gtlqjiuegr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yongpay.top/gtsezbzwaz.html

TS:   constructor(public name: string) {}
来源：http://hz.sweek.top/gtuymykvla.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtgklzqrkf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gtwjshrvyh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gtojfcbhmb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtwegkxltx.html

[G03] 实例属性
来源：http://hz.daria6918.cn/gtqapxwxvw.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtfajshqro.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gtkpdxwars.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtyrctprex.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtmjgvthuc.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtecsnlaqc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtavzmjscj.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gtkzvgeeah.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sweek.top/gtvjjeiaxh.html

[G04] 定义方法
来源：http://hz.pengpengdd.cyou/gtjjkouool.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtaqeubjag.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj202588.top/gthtwlcyxh.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigufen.top/gtcqkmhocm.html

TS:   greet(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtuwvgmftx.html

Java: String greet() { return name; }
来源：http://hz.jinqigufen.top/gtolchxlyv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.c1oappe.top/gtzzzvaknc.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtiphpvydu.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtsgcknuef.html

[G05] 继承
来源：http://hz.ydjk.org.cn/gthnyprwhx.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gtolcrkarq.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtrkpshzcw.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtawyuzwju.html

TS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtfunbqdpd.html


<!-- 参考信息 -->