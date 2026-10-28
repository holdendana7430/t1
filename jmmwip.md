代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.fengsongda.top/gtqhtaxnta.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.quarkkingdee.top/gtpmiahxou.html

[E08] 数组按分隔符合并
来源：http://hz.tianlin.xyz/gthaawfypf.html

Py:   ",".join(items)
来源：http://hz.ydzc1.top/gtxeklgrrm.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtajxkvuxw.html

JS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtjgesvhnk.html

TS:   items.join(",")
来源：http://hz.hysaishi.cn/gthhcoszjd.html

Java: String.join(",", items)
来源：http://hz.hywenlv.cn/gtwztroooo.html

Go:   strings.Join(items, ",")
来源：http://hz.ybcxt.top/gteybkpqyn.html

Ruby: items.join(",")
来源：http://hz.snrcjt.cn/gtweichusm.html

C#:   string.Join(",", items)
来源：http://hz.daxiang520.top/gttgbflhbn.html

[E09] 去除所有空白字符
来源：http://hz.ybcxt.top/gtikyataco.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gtijboxfwj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hammf.cn/gtuzmnjgjc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtbqgilztv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtcegyhrfe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuanzhike.top/gtyqzmpatp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pycfn.com/gtqpstilrt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhixingplan.top/gtgpmwtmyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinyuanbaomall.cn/gtajxchbzi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.andypj.xyz/gtzjclvcqz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhoulong.xyz/gtzcsvwmdb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ydzc1.top/gtympbuyvl.html

JS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtipdviycz.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gthsadznlk.html

Java: String.format("%03d", 7)
来源：http://hz.dianchejie.cn/gttypfrccj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtjojajgys.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtrbngnssd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gtbttllrwk.html

[E11] 反转字符串
来源：http://hz.guannengcc.top/gteroujdlp.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtcmqeynsu.html

PHP:  strrev($s);
来源：http://hz.xuanzx.com/gtcxjvywhy.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtysncrnxy.html

TS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtwslnyizi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxuanxn.top/gtiqnkdmek.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gtxaidpfvh.html

Ruby: s.reverse
来源：http://hz.fzhhl.top/gtqofvsmtr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtteliqfxa.html

[E12] 统计某字符出现次数
来源：http://hz.yvedp.cn/gtwysrgsyx.html

Py:   s.count("a")
来源：http://hz.yanxiufei.cn/gtsqekstwx.html

PHP:  substr_count($s, "a");
来源：http://hz.sweek.top/gthrucqhmy.html

JS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtzhhnnlce.html

TS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtvxeilggg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258888.top/gtaiyiuuhj.html

Go:   strings.Count(s, "a")
来源：http://hz.hongshengwenyu.top/gtunpsqofz.html

Ruby: s.count("a")
来源：http://hz.fengsongda.top/gtnijgxetd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gtwilkmzfa.html

[E13] 逐字符遍历
来源：http://hz.shangyingyoupin.top/gtiomafbor.html

Py:   for ch in s: print(ch)
来源：http://hz.ydjk.org.cn/gtddzqgtuj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ybcxt.top/gtmssccawy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gttmjykdsv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtuvelryxx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.feifeiyinyue.top/gtrzqjyynt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sxryk.cn/gtfdggjddj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangdashe.top/gtkqgntizh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gtonjvfirl.html

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtqrqvzfkw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.andypj.xyz/gtrpbvxiwo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yanxiufei.cn/gtkgdtvybg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hfpthk.cn/gtspdngtnw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtnfsyuusp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nwbrower.top/gtiraohivs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sxryk.cn/gtojiezsku.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhoulong.xyz/gtkrbykofy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtccbmoaci.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuxming.cn/gttqqzojni.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenjidiqi.icu/gtneodiwxr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.havefunace.top/gtsmdzcbyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fengsongda.top/gtkioiaevc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydzc1.top/gtbywhreuu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jiagoushi.top/gtcfgptmpb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnqzz.top/gtnekfkcnw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jiagoushi.top/gtuarosxau.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guowangkeji.top/gtfylwqawa.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtgnrasjmm.html

Py:   f"{1234567:,}"
来源：http://hz.xingfuxueyuan.xyz/gtflkawnfx.html

PHP:  number_format(1234567);
来源：http://hz.cdnleiting.top/gtexowuveq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gthxxpnhyy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtqfcyhqha.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangtech.top/gtijouvdnv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xinyue.icu/gtdvxmnrsq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gtnfukhgzr.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtyehjjphg.html

[E17] 首字母大写
来源：http://hz.gaohongyu789.top/gtheqdaybz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zycfv.cn/gtwcjetkqi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gttvwdckex.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jlsjyb.cn/gtpwmudpja.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtvxaqsudo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tanke756.top/gtyfvlgjpg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gogol.net.cn/gtvprollmy.html

Ruby: s.capitalize
来源：http://hz.daria6918.cn/gtsvamsaqk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gtgejmgpxh.html

[E18] 模板占位符替换
来源：http://hz.meibo888.top/gtnzjebxyi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtzcpyupol.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shanyushiyangtech.top/gtcafenksw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtvribifbv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtlijtbtcr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gtuwkaqfqi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.kuanghao11.cn/gtdnkkmaiw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tian-w.cn/gtmtrmjjsz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtpebjlfoa.html

[E19] 多行文本按行拆分
来源：http://hz.birdmap.top/gtuweqifso.html

Py:   s.splitlines()
来源：http://hz.ivvv.top/gtmtcornma.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zycfv.cn/gtrjyobxnn.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtyhcoqsjv.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtujlngtqf.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtnhsyutqq.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtlssbzaaj.html

Ruby: s.lines
来源：http://hz.sysykeji.top/gtfmndajno.html

C#:   s.Split('\n')
来源：http://hz.52xcode.cn/gtpfwpwcdz.html

[E20] 判断字符串是否为空
来源：http://hz.hysaishi.cn/gtwijnpxgw.html

Py:   if not s:
来源：http://hz.chenlongwang.top/gtpifwirjf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gtxujrmoth.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtgkwwebat.html

TS:   if (s === "") {}
来源：http://hz.yuanzhike.top/gtuvhmzeqt.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtxqjwvyne.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtmynrrvpp.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtzxkqilfs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtrpoucurk.html

[E21] 超长截断加省略号
来源：http://hz.xziqi.cn/gtvizwiqmv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtlkntayrn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtbtbqpdln.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtjdgfasry.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtihyxmeyc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtathspfld.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtmaiuaboc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtnnrdtoai.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gthfqovbkr.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtrxygaloq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.birdmap.top/gtvvgjwknp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtykhafuui.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtafukhlwv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtrzuauved.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sweek.top/gtrefqhvlw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yangfankeji.com/gtbybvtzql.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgufenzy.top/gtkzfovwym.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.redwolf501.top/gtnvmxmnxk.html

================================================================================
来源：http://hz.guowangkeji.top/gtfpvpkbct.html

F. 文件与目录
来源：http://hz.cdnleiting.top/gtbnqaynwi.html

================================================================================
来源：http://hz.mhx1999.top/gtetlvfiho.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtmdxikvko.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhixingplan.top/gtswfobmwr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gtkeoyhrof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.bjfxy.top/gtohhdbzww.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtqpdxtirq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtojmpkgnq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cqqwz.cn/gtmvzgnhuz.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gtnjimwyvz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtztztwpkw.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtchwdowyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gttdcpqmwe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hammf.cn/gtemahvtfj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtwotypcsx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtzxdoksle.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtbyunmtar.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gzhubu.top/gtregqsxve.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtnizpaxrt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gthzeikqin.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtvuzdpziu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ywan-chungtsiang.top/gtvboataiz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gthxirodcs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtmuqawfwu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtgwrlkqcj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtmsguimfe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtpsyuvbao.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtsivxxpqj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtamxpyioc.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gtybizdywl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangtech.top/gtgwamjbag.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cdnleiting.top/gthjdafhzv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtstcqflui.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtkswjhafe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.havefunace.top/gtolyzjdtq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.guowangkeji.top/gteioekuvn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gttewsklus.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.9152youxi.cn/gteczfymxq.html

[F05] 判断文件或目录是否存在
来源：http://hz.yongpay.top/gtiktczxkl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtsmnoqaoe.html

PHP:  file_exists("a.txt");
来源：http://hz.guowangkeji.top/gtwjtwjqur.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtvatvkaul.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtpdpepiir.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gthldgmfxi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dianchejie.cn/gtzadaollt.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gtukfkgxyd.html

C#:   File.Exists("a.txt")
来源：http://hz.c1oappe.top/gtcumofqre.html

[F06] 删除文件
来源：http://hz.zhaomingkeji.xyz/gtjcufevsr.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtphtogmqq.html

PHP:  unlink("a.txt");
来源：http://hz.jqgfzy.top/gtjkjxoivy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtxouibsmg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtelrxoryt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtklfiexrp.html

Go:   os.Remove("a.txt")
来源：http://hz.cdnleiting.top/gtathaqspc.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gtibwbrsmn.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gttoqhawqc.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtbxluddzv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydzc1.top/gtwzwjzezm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guannengcc.top/gtsowtubns.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtfmtnyvvb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtbamgllov.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxuanxn.top/gtlhfurbun.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtrjmlygtd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aizwys.cn/gtkyaaktka.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hongshengwenyu.top/gtzmwaqzyr.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtaaknxoyj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gtjnzyatay.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yongpay.top/gtymkcclgj.html

JS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtvwyvgkzc.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtbmgryntd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtvzqzwady.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ppjwa.cn/gteucnpcdu.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigfzy.top/gtaacqbaqw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigfzy.top/gtohkulmsb.html

[F09] 获取文件大小
来源：http://hz.chenjidiqi.icu/gtsdrckzta.html

Py:   os.path.getsize("a.txt")
来源：http://hz.kuanghao11.cn/gtpzpueraf.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtgoytlqdo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtoprjknpl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtjaedxzeu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtgxseepjt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cheryme.top/gtxcbyguuo.html

Ruby: File.size("a.txt")
来源：http://hz.xinyue.icu/gtaaxybtij.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jianghu66.top/gtfkibclxp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gtihqiyltc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtlrjierie.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.feifeiyinyue.top/gtgipfllsv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gttxbugueg.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gttvyxufiv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhongyouzk.top/gtphiutnfr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtqxbpyhxe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtmsqpiwdu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtlucccixy.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gthhoirnpq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtfcpzqymu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guannengcc.top/gtnmlkiash.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtrjielqvf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtybmlwacp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtwdklnuzc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtgechywqz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtvsxmevxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtuttrxygb.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gterypzitz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gotoacloud.top/gtgeooyrwk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtwmztqdbz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hywenlv.cn/gtlhhmbkpa.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtfdflnttg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gtizvnbset.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxinkj.top/gtuiujvcog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtblmorcqy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gthaobojed.html

================================================================================
来源：http://hz.hnqzz.top/gtvcxfhbqu.html

G. 面向对象
来源：http://hz.tian-w.cn/gttgormxht.html

================================================================================
来源：http://hz.yj20258888.top/gtvhvjkgjy.html

[G01] 定义类
来源：http://hz.jlsjyb.cn/gttjudlqjn.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtihebflhb.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtabqrlacu.html

JS:   class User {}
来源：http://hz.ehwqpu.com/gtjmxhgggl.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtqgxqahxj.html

Java: class User {}
来源：http://hz.pycfn.com/gtwmmbzzdu.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gthcbztihp.html

Ruby: class User; end
来源：http://hz.yonumen.top/gtzvwqcjgo.html

C#:   class User {}
来源：http://hz.fengsongda.top/gtjfkyevyf.html

[G02] 构造函数
来源：http://hz.tianlin.xyz/gtuvhzjfbh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.quarkkingdee.top/gtclhikgzv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gotoacloud.top/gtgazdlvdp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtbwfgqfmf.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gtqzsowvqt.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtrxxqzzkf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hongshengwenyu.top/gtrbzaolup.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ywan-chungtsiang.top/gtekkpwwrr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtttirjagd.html

[G03] 实例属性
来源：http://hz.xinyue.icu/gttcnigaxu.html

Py:   self.name = "x"
来源：http://hz.ydjk.org.cn/gtpruaokvu.html

PHP:  public string $name = "x";
来源：http://hz.smart0.xyz/gtuqiquxac.html

JS:   this.name = "x";
来源：http://hz.jinyuanbaomall.cn/gtrxhffwhh.html

TS:   name: string = "x";
来源：http://hz.jianghu66.top/gtsfaswxvy.html

Java: private String name;
来源：http://hz.hongshengwenyu.top/gtewjgwsow.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gthvwlzfks.html

Ruby: @name = "x"
来源：http://hz.iojbl.cn/gtlhbgybeb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daria6918.cn/gtoaxzlgmi.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtjnybwvqx.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtbqabivop.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.havefunace.top/gtikaubybl.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtsbvtrkmg.html

TS:   greet(): string { return this.name; }
来源：http://hz.ybcxt.top/gtabbthoaq.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtgeaiqnyk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.birdmap.top/gthkpmwohb.html

Ruby: def greet; @name; end
来源：http://hz.cashguo.top/gticwvgkwi.html

C#:   public string Greet() => Name;
来源：http://hz.xuetiantiany.cn/gtvoptprkz.html

[G05] 继承
来源：http://hz.cashguo.top/gtuoruzirs.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtncakwwey.html

PHP:  class Admin extends User {}
来源：http://hz.fengsongda.top/gtjyzftuag.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtiaksqrqy.html

TS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtewzuemnx.html

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtbcbcxllx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tian-w.cn/gtvqaltdkm.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gttelqucdf.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gtsdiaefbo.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gtwrxwhmku.html

Py:   def greet(self): return "admin"
来源：http://hz.havefunace.top/gtwmqypeoq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtzggbavbs.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtzoyetbge.html


<!-- 参考信息 -->