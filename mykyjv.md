代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.chenlongwang.top/gtpevkdhmg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shangyingyoupin.top/gttihlpevg.html

[E08] 数组按分隔符合并
来源：http://hz.jinyuanbaomall.cn/gtkmprqcpr.html

Py:   ",".join(items)
来源：http://hz.jlsjyb.cn/gtjdgqrgcd.html

PHP:  implode(",", $items);
来源：http://hz.daria6918.cn/gtrghclkyg.html

JS:   items.join(",")
来源：http://hz.daxiang520.top/gttmyiuise.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtnxrbjsdi.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gttdiptkiw.html

Go:   strings.Join(items, ",")
来源：http://hz.xziqi.cn/gtzwymtscx.html

Ruby: items.join(",")
来源：http://hz.yj20258.top/gtyhswvvip.html

C#:   string.Join(",", items)
来源：http://hz.cheryme.top/gtodftccyr.html

[E09] 去除所有空白字符
来源：http://hz.fzhhl.top/gtymdmsoom.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtqiyiepqp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtgxsogwzk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtwjchqded.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtzfubxssj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jiagoushi.top/gtifglaair.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenlongwang.top/gtlzymlgks.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gtbmejtuoz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dianchejie.cn/gtmjledyen.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shuidangran.top/gtpihtqlud.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuetiantiany.cn/gtyihrzxlv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tianlin.xyz/gtsxdutnru.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtkafwefzg.html

TS:   "7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtbqpgsjqn.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtwesuhuzm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtuilrfrdy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtppdpzttc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangdashe.top/gtecccxwti.html

[E11] 反转字符串
来源：http://hz.guowangkeji.top/gttcygrujd.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtlwcdmevg.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtoxqdhzdu.html

JS:   [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtebukkhmd.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gttyxbxuxf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtbubiehsp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtymslzwam.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtnndoyhvt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtlxjkfxvr.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gtnpreuqzv.html

Py:   s.count("a")
来源：http://hz.feifeiyinyue.top/gtphkhrtuq.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gtbsgyegvf.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtrnivxqrl.html

TS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtqeoyyogb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.vqdsnc.cn/gtxqryczen.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gtemxeojbi.html

Ruby: s.count("a")
来源：http://hz.fengsongda.top/gtjtxqhplh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtsvicmrjt.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gtqftgiqvt.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gtrmvmflyw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.havefunace.top/gtldoywdus.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtyfdlzllo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtykkenywz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.meibo888.top/gtbspknppx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtvczwqqjb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtiaxozssd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sufxvd.cn/gtwcheswot.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtubzwylfu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hysaishi.cn/gtbmoizorb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtawlkabao.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtervdlblp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zdqjudy.top/gtqyjbgmst.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenjidiqi.icu/gtbwpeuxqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dianchejie.cn/gtwhqbpsmr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cucudq.cn/gtvyqarmnj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pengpengdd.cyou/gttyqmnmlk.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtfbjpiacn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydzc1.top/gthypzumei.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtuftaxjac.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xingfuxueyuan.xyz/gtiqxudyzo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ppjwa.cn/gttdxuemfu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fengsongda.top/gtoucwfrix.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gtfabyaafi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gtnvinkeci.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aibaodan.cn/gtwdsumuke.html

[E16] 数字千分位
来源：http://hz.yuanzhike.top/gtgshasddx.html

Py:   f"{1234567:,}"
来源：http://hz.pengpengdd.cyou/gtfuoxyaux.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtbsyjuavz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtxmsfczls.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtohsfgvtv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhengqikj.top/gtuhyhgkvl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daria6918.cn/gtoyykacmh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xylfe.cn/gttxctwymc.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtkdhnxxmy.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtmywquhze.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ybcxt.top/gtnetmmnij.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gtjhlbfhnp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gtubzolaxc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtnudnyggp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtycazylnk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gtwbawkyog.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gtzhyaiqxj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.quarkkingdee.top/gtfufuccch.html

[E18] 模板占位符替换
来源：http://hz.hfpthk.cn/gtzwrjzmru.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.bjfxy.top/gtjiypdqpz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gtquopupul.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtgketlxir.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtgyynkxav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gtalbglwoz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtegrjgrim.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.svipenyu.cn/gtqqhpfokq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtkxotzqiv.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gtwcaqijab.html

Py:   s.splitlines()
来源：http://hz.zhoulong.xyz/gtbykedxzp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gttiahcrag.html

JS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtdnwoqykk.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtgntxxemi.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtntjuctno.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gttryfkzyz.html

Ruby: s.lines
来源：http://hz.fengsongda.top/gtmsrtbswm.html

C#:   s.Split('\n')
来源：http://hz.pycfn.com/gtjjvazeev.html

[E20] 判断字符串是否为空
来源：http://hz.jyoumei.cn/gtmmopxsgy.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtpmjwttdc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtsllpzmcl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtawhxlsdh.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtsrqsyggb.html

Java: if (s.isEmpty()) {}
来源：http://hz.c1oappe.top/gtvcnhxezw.html

Go:   if s == "" {}
来源：http://hz.xziqi.cn/gtlchozvwy.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtttbftprb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zycfv.cn/gtrjmxxmdz.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gthxvpklgu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnqzz.top/gtrybslwfb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtjkwxtfst.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtlwrjrgfa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtdgjjkkjd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtdwakjicd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtfuyikyvx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gtahzbiteb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gttlcuowxd.html

[E22] 字节长度与字符长度
来源：http://hz.tian-w.cn/gtikkxdzim.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gtmhaptcry.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtigimlsru.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtbfifimnw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtprwzwygo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtlhsabloq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gtwdaqsmdy.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gtygtdsovz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gtmjqfshvf.html

================================================================================
来源：http://hz.pycfn.com/gtonlbdskg.html

F. 文件与目录
来源：http://hz.ybcxt.top/gtouobfyej.html

================================================================================
来源：http://hz.yongpay.top/gtxskbgogs.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gtcnrwwlwc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtfltsdzbo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yangfankeji.com/gtpyiipgdx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sweek.top/gtwtrpewnq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigufen.top/gtkfrnxkxq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtulyroiql.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenzaomai.com/gtutfwqhbw.html

Ruby: File.read("a.txt")
来源：http://hz.svipenyu.cn/gtbjnmqrke.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtatdpxwxp.html

[F02] 逐行读取文件
来源：http://hz.bjfxy.top/gtwvqfubbh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ivvv.top/gtjgzhpqzo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aizwys.cn/gtcphbzwbf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtgtdfzwvp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtnyfdyubi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtxdxrkuvd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pengpengdd.cyou/gttnmctnri.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zdqjudy.top/gtruojocxw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtlwgohtct.html

[F03] 写入文件（覆盖）
来源：http://hz.0kj1m.cn/gtdhqtvqho.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xingfuxueyuan.xyz/gtwzvzqaqz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtdwneqdls.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtmmrodjia.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtheyozhtm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinghuilouyu.cn/gthwfocjwd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hysaishi.cn/gtukdtsdnb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtejodydnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydzc1.top/gtjczugwsh.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtdbwtewzb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xinyue.icu/gtmnkcaizw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yangfankeji.com/gtutzzijwl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtuhoxrxch.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtjjrfxhgn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtrzlwlpcf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cdnleiting.top/gtgylwzaae.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gthevrchox.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtwbcorlrj.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtpfwflyqz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gthbzfcvqg.html

PHP:  file_exists("a.txt");
来源：http://hz.cqqwz.cn/gtbaosnmfo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtgbpxxezz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtfsfcotwx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtsqdopwwb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtougucrqy.html

Ruby: File.exist?("a.txt")
来源：http://hz.fzhhl.top/gtclqnomtd.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtbsekeezh.html

[F06] 删除文件
来源：http://hz.yuxming.cn/gtyjukrtrw.html

Py:   os.remove("a.txt")
来源：http://hz.ehwqpu.com/gtszposwah.html

PHP:  unlink("a.txt");
来源：http://hz.nwbrower.top/gtxpljaois.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtcteusyrq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtisvobets.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtbbgffqay.html

Go:   os.Remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtnjfwulna.html

Ruby: File.delete("a.txt")
来源：http://hz.sxryk.cn/gtjfmgdmwu.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtpmntcyzb.html

[F07] 创建目录（含多级）
来源：http://hz.hammf.cn/gtnvkbnlol.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.meibo888.top/gtcrexsfhq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtxotiqzqo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtattdlvps.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtzktpzfpl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtsvcnhfrb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yongpay.top/gtgawyxcbd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sweek.top/gttdwrnedi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.316326.xyz/gtymfqnkom.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gtqbmlugky.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gtbdqtlpdg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtqlxrpbwk.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gthxmmuymf.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtrmfrupch.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtgilqzrze.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtzgjnetkh.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gtyebwscpg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuanzhike.top/gtjivnvxxh.html

[F09] 获取文件大小
来源：http://hz.zhaomingkeji.xyz/gtucbqfwki.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daxiang520.top/gtracfbtfl.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtnfnfagjy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtwuvseiif.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gttdajwxny.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtaysfwgoi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daria6918.cn/gtjwtsxwze.html

Ruby: File.size("a.txt")
来源：http://hz.hysaishi.cn/gtotrtoioy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtkkhaddjp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtdxajuzcj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtwjdbrobr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.c1oappe.top/gtnfskudst.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtixhakzfn.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtlralskfv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgufenzy.top/gtmijrsitz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ehwqpu.com/gtozmqnknj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtraqgyaok.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhixingplan.top/gttyppsogi.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtcrmpvsbn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtnhgddsoh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guannengcc.top/gtwmdjvykj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtbsgzgqij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtkczlmpdz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tianlin.xyz/gtdiiugchf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhengqikj.top/gtlgqdjlhl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtgagmbfzh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gtiqtjczgb.html

[F12] CSV 读写
来源：http://hz.cdnleiting.top/gtuhouxeql.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yueranfly.top/gtzoouauuu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sysykeji.top/gtrokejwfw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sxryk.cn/gtzuucokrs.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtflkhblks.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtsjdeowhe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gtlhxsexoe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gttzodkjro.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhixingplan.top/gtkvjkgetl.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgjpqyfiw.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gttaoissdu.html

================================================================================
来源：http://hz.aizwys.cn/gtueompxzu.html

[G01] 定义类
来源：http://hz.shzxlz.cn/gttdgdtrow.html

Py:   class User: pass
来源：http://hz.feifeiyinyue.top/gtwethlnvg.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtntlorvax.html

JS:   class User {}
来源：http://hz.yuxming.cn/gtzuuiisdo.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gtyinhnguo.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtrefppwim.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtbvoqeubh.html

Ruby: class User; end
来源：http://hz.xylfe.cn/gtvadzuaur.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtfqfcsmbr.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtnfnqkbus.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhaomingkeji.xyz/gtrtzdnvmr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tanke756.top/gtzbruxhsx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtvxqqgmxl.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gthqngeipe.html

Java: User(String name) { this.name = name; }
来源：http://hz.daxiang520.top/gtngfmutfg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtxgmepiso.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtppawqnct.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gtwoictmgy.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtohayrywb.html

Py:   self.name = "x"
来源：http://hz.cashguo.top/gtofmdmkhl.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtefugqnzf.html

JS:   this.name = "x";
来源：http://hz.guowangkeji.top/gtroyzykdq.html

TS:   name: string = "x";
来源：http://hz.jqgufenzy.top/gtmmrofwve.html

Java: private String name;
来源：http://hz.jianghu66.top/gtclqzmpir.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gtffspdcwz.html

Ruby: @name = "x"
来源：http://hz.ehwqpu.com/gttkryxchw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtxiqlyroz.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gtanopvifh.html

Py:   def greet(self): return self.name
来源：http://hz.smart0.xyz/gtteznwimt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtghpbodtd.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtsidpeeax.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtfncetkoa.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtaobbcnom.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cqqwz.cn/gtijelkjdr.html

Ruby: def greet; @name; end
来源：http://hz.hywenlv.cn/gtrbrjtjfu.html

C#:   public string Greet() => Name;
来源：http://hz.hongshengwenyu.top/gtuwvvlgkt.html

[G05] 继承
来源：http://hz.daria6918.cn/gtvdjeqnjl.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtgnytflrl.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtkeuzyrox.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtyegkotkg.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtanngmxbk.html

Java: class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtjdcoorfv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtkzpbumgw.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtagmfvgnj.html

C#:   class Admin : User {}
来源：http://hz.jyoumei.cn/gtlixphetp.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtaaegcvmm.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gtqfmdxibs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtrhvthacf.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtgqgqnaes.html


<!-- 参考信息 -->