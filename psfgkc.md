代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtjuqtgfmm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtoncnnlhi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtyawqszzv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yanxiufei.cn/gtmvbepzxm.html

C#:   s.Replace("a", "b")
来源：http://hz.hnqzz.top/gtppawxkut.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtfbiyyfkc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtxtlasyrb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gtcdvkflbe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhijiandao.cn/gtslogzrqv.html

TS:   s.split(",")
来源：http://hz.shzxlz.cn/gtemtgseie.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtjwwagvud.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gtmerauuif.html

Ruby: s.split(",");  s.split
来源：http://hz.jqgfzy.top/gtinghzbrj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daria6918.cn/gtuygwcsax.html

[E08] 数组按分隔符合并
来源：http://hz.ydzc1.top/gtbbgbuezn.html

Py:   ",".join(items)
来源：http://hz.jinghuilouyu.cn/gtoyvsuchj.html

PHP:  implode(",", $items);
来源：http://hz.zhijiandao.cn/gtjliyshgj.html

JS:   items.join(",")
来源：http://hz.zhengqikj.top/gtyehoxpdl.html

TS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtzgpojxck.html

Java: String.join(",", items)
来源：http://hz.jinghuilouyu.cn/gtqwpemmln.html

Go:   strings.Join(items, ",")
来源：http://hz.dashuyun.cn/gttuknkrct.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gtngrorkhg.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gttwodkeyh.html

[E09] 去除所有空白字符
来源：http://hz.tianlin.xyz/gtrzihscpq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtougtzgch.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhijiandao.cn/gttbwgmxef.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtphrxlixd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtvoxytsru.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gteyxbgvbb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.meibo888.top/gtzsynjqim.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtpmkznwhr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hysaishi.cn/gtihxmjeuo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jyoumei.cn/gtysaahrvm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuxming.cn/gtszcwwjem.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtujikgrno.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtrfkgnjsf.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtromxdlif.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtqtjimuay.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yvedp.cn/gtxpptpxrc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ybcxt.top/gtgdegwcez.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangtech.top/gtmilvoasm.html

[E11] 反转字符串
来源：http://hz.xuanzx.com/gtqpnpegep.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtocxgjtqx.html

PHP:  strrev($s);
来源：http://hz.guowangkeji.top/gtxsrnbifh.html

JS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtyxpwbluj.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtfbugidfw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jiagoushi.top/gtsykgruid.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258.top/gtmditfdsm.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gtrmsfvmph.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtzxxchteb.html

[E12] 统计某字符出现次数
来源：http://hz.tanke756.top/gtxyqnskov.html

Py:   s.count("a")
来源：http://hz.jqgufenzy.top/gtofhxicha.html

PHP:  substr_count($s, "a");
来源：http://hz.ivvv.top/gtpkdfyurp.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtkdzlknbd.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtesgwfked.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fzhhl.top/gtexvtrhon.html

Go:   strings.Count(s, "a")
来源：http://hz.tanke756.top/gtdquwpgkr.html

Ruby: s.count("a")
来源：http://hz.yuxming.cn/gtwbgwmwxy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtehkuooga.html

[E13] 逐字符遍历
来源：http://hz.gotoacloud.top/gtoihvvoch.html

Py:   for ch in s: print(ch)
来源：http://hz.sufxvd.cn/gtynawdjyf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.havefunace.top/gtpdmmkxwb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtwjxhoxtg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cashguo.top/gtdmyorkyx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sysykeji.top/gtzyargrxs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ehwqpu.com/gtvccfehig.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gtmprsomjj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daxiang520.top/gtagnaxzub.html

[E14] URL 编码与 Base64
来源：http://hz.zhoulong.xyz/gtccaukjjz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sufxvd.cn/gtbullepkr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhixingplan.top/gtdfzacglg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtxmxlscdz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shuidangran.top/gtepkiylcc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.redwolf501.top/gtuzlauido.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.feifeiyinyue.top/gtwzrcfjxj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtlzfnhord.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtkonludvh.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtpvmcuohn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ppjwa.cn/gthykatyjh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.bjfxy.top/gttzdsbakh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gttmpzbkpw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shangyingyoupin.top/gtipkxceqi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhijiandao.cn/gtfqsgyehb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtoaezybkb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.vqdsnc.cn/gtnorcjrbw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gaohongyu789.top/gtfgpdhgue.html

[E16] 数字千分位
来源：http://hz.fengsongda.top/gtefyavbut.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtuqhkonta.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtsrrywsdv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtyakmrfmk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtahuqfbau.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hywenlv.cn/gtrvbbfikn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtmibsmeni.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.snrcjt.cn/gtunbqicwd.html

C#:   1234567.ToString("N0")
来源：http://hz.chenzaomai.com/gtxdquoone.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtjrarkxki.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pycfn.com/gtaqjvdujq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shanyushiyangtech.top/gtjqhbemip.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtgqrknqtq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtooexpwii.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtmeoftgzx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gtrkmcnfrs.html

Ruby: s.capitalize
来源：http://hz.sysykeji.top/gtkwkpdsmz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cdnleiting.top/gtjxwbdxfe.html

[E18] 模板占位符替换
来源：http://hz.ydjk.org.cn/gtjwzxqlwy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinqigufen.top/gtivfqmmsq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aibaodan.cn/gtcectwkmw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtkabzvtcq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtpnbbwqro.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gtluewzxod.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhoulong.xyz/gtsoabmbiq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtdlwefuex.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtmrcdaskx.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtmotlqceb.html

Py:   s.splitlines()
来源：http://hz.0kj1m.cn/gtyvdeggda.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenzaomai.com/gtnwruiuia.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtrajvnzsp.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtedfvfuex.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtrrykdazy.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gttvcydtdb.html

Ruby: s.lines
来源：http://hz.zhongyouzk.top/gtiegcdefh.html

C#:   s.Split('\n')
来源：http://hz.meibo888.top/gtvglvpzlr.html

[E20] 判断字符串是否为空
来源：http://hz.zhengqikj.top/gtvqdshzfw.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtesfvewgr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinghuilouyu.cn/gtqlsbvwrd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuanzhike.top/gtkkxyobci.html

TS:   if (s === "") {}
来源：http://hz.bjfxy.top/gtmluzgucu.html

Java: if (s.isEmpty()) {}
来源：http://hz.zdqjudy.top/gtqvwurzdp.html

Go:   if s == "" {}
来源：http://hz.shuidangran.top/gtchhgocmf.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtpwwnaoec.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtnmktqxzk.html

[E21] 超长截断加省略号
来源：http://hz.ydzc1.top/gtanprxcff.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtvbphfpuv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yvedp.cn/gtokymzuet.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtbxfsjtww.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtbdjnlsih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtwqcboqro.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtransjjda.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guannengcc.top/gtfonigkfw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtmguaajwi.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtbmmclhsp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gtjmpfcael.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gttrckmkrg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtuftxirnj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gtriqqctjv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gotoacloud.top/gtrwpbazwc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hfpthk.cn/gtxszecaza.html

Ruby: s.bytesize;  s.length
来源：http://hz.jianghu66.top/gtllzpfjmz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtlaxwpuce.html

================================================================================
来源：http://hz.sxryk.cn/gtmsbqqljc.html

F. 文件与目录
来源：http://hz.meibo888.top/gtxxfovwdx.html

================================================================================
来源：http://hz.chenlongwang.top/gthbahomuc.html

[F01] 读取整个文件
来源：http://hz.zhaomingkeji.xyz/gtcmqlzlgn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.9152youxi.cn/gtieuoncrg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinghuilouyu.cn/gtbhicqbfw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghu66.top/gtqprnkuxd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.havefunace.top/gtwmxnzpsu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtexhzdosy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxinkj.top/gtwlcinhxm.html

Ruby: File.read("a.txt")
来源：http://hz.xinyue.icu/gtrvzwkexj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gtftvtamrz.html

[F02] 逐行读取文件
来源：http://hz.yuxming.cn/gtkklkjkpq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yueranfly.top/gtfuoitniw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gthdspjtiy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtgvklhujm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtdbpaegro.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtmuezqpuc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tian-w.cn/gthgvdgzyw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuxming.cn/gtzdreskvs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zdqjudy.top/gtygxyilcx.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtubboevri.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cashguo.top/gtrrdiwoat.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtxzqbcwxt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtrnpejdgx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtrhzxfcxy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtoposgqrb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.9152youxi.cn/gtyohqzzzo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gtsqrlytpk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gtdqwmzcui.html

[F04] 追加写入文件
来源：http://hz.xuetiantiany.cn/gtamnrcupe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtvtvrusjw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigufen.top/gtzphexkge.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtrpdqmtoc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtptdiypem.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xziqi.cn/gtmqrllopq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtotswdmxa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtsjmxfgvq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnxiangtu.top/gthkkilslg.html

[F05] 判断文件或目录是否存在
来源：http://hz.yonumen.top/gtntgxkwro.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.birdmap.top/gtxkezdvoo.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtinwuhlxz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtcgfkxusr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtfhvozzlz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtjhnndicj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gtakkwhzct.html

Ruby: File.exist?("a.txt")
来源：http://hz.gogol.net.cn/gtstspikkm.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gtllpmpkdi.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtasrweszd.html

Py:   os.remove("a.txt")
来源：http://hz.zhijiandao.cn/gtlceneigj.html

PHP:  unlink("a.txt");
来源：http://hz.aizwys.cn/gthzkavawx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtkdjuxwba.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtballuicc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtxldbriyn.html

Go:   os.Remove("a.txt")
来源：http://hz.cucudq.cn/gtluebxvtc.html

Ruby: File.delete("a.txt")
来源：http://hz.feifeiyinyue.top/gtxnvsxhqm.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gtpazvhjgv.html

[F07] 创建目录（含多级）
来源：http://hz.nanxuanxn.top/gtvqjosmim.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgfzy.top/gtpfucrhvs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.kuanghao11.cn/gtmhbgpzbg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtvenhswhv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtxbayuapb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yangfankeji.com/gtwnkpeqrm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aibaodan.cn/gtvozyswoc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydzc1.top/gtfwqagtam.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gtuoisnfmf.html

[F08] 遍历目录
来源：http://hz.yvedp.cn/gtshzvfsdi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtodhnritw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.quarkkingdee.top/gtopivtuzg.html

JS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtlwuhcoqf.html

TS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtvmnvkxrk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtxffhhtxi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtxxwbjxhd.html

Ruby: Dir.children("dir")
来源：http://hz.quarkkingdee.top/gtofkwkttg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yongpay.top/gtxsfszgxk.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtgrhcffer.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtwchlhfpg.html

PHP:  filesize("a.txt");
来源：http://hz.jlsjyb.cn/gtkdgnjlyq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtibbxxdab.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtlwvvrqnx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtkcrxsyhl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jianghu66.top/gtqchzlbqz.html

Ruby: File.size("a.txt")
来源：http://hz.jlsjyb.cn/gtxfzmpgbs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gthdkuykfm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gogol.net.cn/gtkrwiigau.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtqkqxvckp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shzxlz.cn/gtoemxfytv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtapgkneza.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtdfccxkrs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gtokuvirpf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yueranfly.top/gtgfkxisqb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtufdwfwus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtxuzwgutv.html

[F11] 复制与移动文件
来源：http://hz.zhongyouzk.top/gtnjxckhdh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtwtmtodhs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenlongwang.top/gtsclgkncb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtmzlfwfnz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtqfntxpvo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cashguo.top/gtfgqgabzz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhixingplan.top/gtdhflcbbo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtiofuukez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.quarkkingdee.top/gtxsveqzcd.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gtjmsjfrvx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhongyouzk.top/gtyxkcgjzw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhoulong.xyz/gtqmvherwn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtbdgqlxsr.html

TS:   // 同上
来源：http://hz.yuxming.cn/gtaysyqngl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jyoumei.cn/gtosovbelq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuxming.cn/gtjtyffnxe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtnmjjggye.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtsjwtppbq.html

================================================================================
来源：http://hz.gzhubu.top/gtygrkbgxs.html

G. 面向对象
来源：http://hz.yueranfly.top/gtiddzodza.html

================================================================================
来源：http://hz.cashguo.top/gtxlbzsbym.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtllzxwznq.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtqnrwaumu.html

PHP:  class User {}
来源：http://hz.aibaodan.cn/gtqbehfozl.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtvutlhxdj.html

TS:   class User { name: string = ""; }
来源：http://hz.xuanzx.com/gtvqzwidcx.html

Java: class User {}
来源：http://hz.smart0.xyz/gtioqrtsqh.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtqbfsgzfz.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtjiwmdgnw.html

C#:   class User {}
来源：http://hz.xziqi.cn/gtscdaqhmz.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtlffkwaxx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gaohongyu789.top/gtllokkuqd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydzc1.top/gtrkwhtesn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtxflizput.html

TS:   constructor(public name: string) {}
来源：http://hz.andypj.xyz/gtitevnkrd.html

Java: User(String name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtwpkwtbtw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ppjwa.cn/gtbnznpxdz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cqqwz.cn/gtzcbtchdp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinyuanbaomall.cn/gtoxqcrpsf.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gtcdyxlaft.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtjxewlamb.html

PHP:  public string $name = "x";
来源：http://hz.9152youxi.cn/gtnvsetadk.html

JS:   this.name = "x";
来源：http://hz.ywan-chungtsiang.top/gtvmrwhhxd.html

TS:   name: string = "x";
来源：http://hz.ydzc1.top/gttpmzttcx.html

Java: private String name;
来源：http://hz.pengpengdd.cyou/gtmlvgrjnj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtluguiduh.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gteuedrwlm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gthhpgmpyx.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtpuhgdvre.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtesgpyudh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtkyyajksm.html

JS:   greet() { return this.name; }
来源：http://hz.pycfn.com/gtfgbjumxv.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtwarlsvcx.html

Java: String greet() { return name; }
来源：http://hz.wangdashe.top/gthndsqncv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.svipenyu.cn/gtgiotyeov.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gttatfclrb.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtybecmtyp.html

[G05] 继承
来源：http://hz.yvedp.cn/gtbmzinnku.html


<!-- 参考信息 -->