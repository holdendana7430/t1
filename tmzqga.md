代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtgborjbbn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtlyjaozdu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hysaishi.cn/gttufrdtco.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtrsfgmbau.html

C#:   s.Replace("a", "b")
来源：http://hz.shzxlz.cn/gtfwafwyyg.html

[E07] 按分隔符拆分
来源：http://hz.xuanzx.com/gtzluyopnd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jyoumei.cn/gtvebouzdn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtnpfujhok.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtlspzdwer.html

TS:   s.split(",")
来源：http://hz.shuidangran.top/gtraowndyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xziqi.cn/gtvovucmfj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhengqikj.top/gtrpyratie.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gthvafahfv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gthwkkkylf.html

[E08] 数组按分隔符合并
来源：http://hz.jinqigfzy.top/gtaamvlaae.html

Py:   ",".join(items)
来源：http://hz.xingfuxueyuan.xyz/gtqvunfbtn.html

PHP:  implode(",", $items);
来源：http://hz.yangfankeji.com/gtztsbaqls.html

JS:   items.join(",")
来源：http://hz.nanxinkj.top/gttrkacryi.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtvcyutrza.html

Java: String.join(",", items)
来源：http://hz.cqqwz.cn/gtfhtdqofi.html

Go:   strings.Join(items, ",")
来源：http://hz.yuanzhike.top/gtsblobshh.html

Ruby: items.join(",")
来源：http://hz.yuanzhike.top/gtrnizhslu.html

C#:   string.Join(",", items)
来源：http://hz.yuxming.cn/gtctkoakur.html

[E09] 去除所有空白字符
来源：http://hz.birdmap.top/gtsorkaioh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gotoacloud.top/gtjgtifwjd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydjk.org.cn/gtwkdzdyfy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gttbxcgors.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtlhiguaus.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pengpengdd.cyou/gtgbzpwrzo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtnayjpybz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydzc1.top/gtfcrbmyek.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtmvtrhxhq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258888.top/gttuzqxvau.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.smart0.xyz/gtwdzfpqjm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aibaodan.cn/gtzhvihwbx.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtftzvrfsl.html

TS:   "7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtgcumtthc.html

Java: String.format("%03d", 7)
来源：http://hz.tianlin.xyz/gtwoqasyhr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.haohaochexian.top/gtkpttilox.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258.top/gtuqmfwuqr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ppjwa.cn/gtnqhtadxs.html

[E11] 反转字符串
来源：http://hz.wangshuangyany.cn/gtczvojqia.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtebjmmlzy.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtnnwkzafy.html

JS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtpmautmjg.html

TS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtafhumqsx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fzhhl.top/gtvhxklupj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtnqwcxrrx.html

Ruby: s.reverse
来源：http://hz.hongshengwenyu.top/gtwskmyjdv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtarfilwjt.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtpaljfgtj.html

Py:   s.count("a")
来源：http://hz.pengpengdd.cyou/gtshllsqfl.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtjpwuzkke.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtmnoxzdvm.html

TS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtzqbzwssb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.birdmap.top/gtwsgfwpdr.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gtgfscduot.html

Ruby: s.count("a")
来源：http://hz.nanxuanxn.top/gtaynkvsqw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtavgzkhzs.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtwgytqszg.html

Py:   for ch in s: print(ch)
来源：http://hz.jlsjyb.cn/gtbgtaqrin.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtdovccits.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtntnqkjze.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtvkpfjnge.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pycfn.com/gtuphypzxf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.316326.xyz/gtbzbjcaes.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gttzebkuzb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtcdelfnkd.html

[E14] URL 编码与 Base64
来源：http://hz.birdmap.top/gtpmzotnfe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tian-w.cn/gtmyjpbbiy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtwprazwfh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.havefunace.top/gtyhgpnavb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgfzy.top/gtyzdbnhel.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sxryk.cn/gtvwbsodjc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhaomingkeji.xyz/gtunvbvegl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuanzx.com/gthuczmrgb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtjeeoyxdb.html

[E15] HTML 转义 / 反转义
来源：http://hz.tianlin.xyz/gtfiiulpso.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj202588.top/gtedaxhvis.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cucudq.cn/gtragqzqas.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ivvv.top/gtarwzpjhx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gtzwlottzy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gtlphmtryc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtmsekarms.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhixingplan.top/gtoltbitjg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gtawbzonie.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtkqynfehd.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtvhctxsbw.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtualpijpa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtwtoecwsz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtvkgzodxt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtyeriiuel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtegpbdiij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.feifeiyinyue.top/gtxcystkua.html

C#:   1234567.ToString("N0")
来源：http://hz.hnqzz.top/gtuhldvpdk.html

[E17] 首字母大写
来源：http://hz.cucudq.cn/gtbhxodsxm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtmddocejs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gthjhwznxy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtzvgickzn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtihnyhwds.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtooiisrzz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gthyowattb.html

Ruby: s.capitalize
来源：http://hz.316326.xyz/gtgcmkuemi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gzhubu.top/gtfbwcpwyc.html

[E18] 模板占位符替换
来源：http://hz.ivvv.top/gtaovrtzyc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuxming.cn/gtspgtunfi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuanzhike.top/gtlvbaggrb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtghhmonpp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtjnkntkqt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhoulong.xyz/gtmriselgs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hfpthk.cn/gtswzunijo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gtqrsjuhiu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xinyue.icu/gtuwcpughx.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtyfmxqnpt.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtmumsvfgl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinyuanbaomall.cn/gtbpxhfgtl.html

JS:   s.split(/\r?\n/)
来源：http://hz.c1oappe.top/gtdfapsxnd.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtcfdgdbaw.html

Java: s.lines().toList()
来源：http://hz.zhengqikj.top/gtxmtiqdqj.html

Go:   strings.Split(s, "\n")
来源：http://hz.gogol.net.cn/gtgnuojagj.html

Ruby: s.lines
来源：http://hz.birdmap.top/gtnussmfkk.html

C#:   s.Split('\n')
来源：http://hz.jqgfzy.top/gtpxsaqhvd.html

[E20] 判断字符串是否为空
来源：http://hz.pengpengdd.cyou/gtgoajqntu.html

Py:   if not s:
来源：http://hz.yj20258.top/gtajpjwdcr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnxiangtu.top/gtixesqjiq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aizwys.cn/gtmzxrldsq.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtarypqlga.html

Java: if (s.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtlopvpajz.html

Go:   if s == "" {}
来源：http://hz.jlsjyb.cn/gtykyybcgh.html

Ruby: if s.empty?
来源：http://hz.cucudq.cn/gtxjfxoamr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gtbiynuwxo.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtwmuqwgcj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangshuangyany.cn/gtjzpkoqvz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtgovlqwuu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtazyhuibk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtmojzurdq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtgwozaofo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigufen.top/gtbcokptsk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgufenzy.top/gtuaqebsrc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gtungpvunl.html

[E22] 字节长度与字符长度
来源：http://hz.shangyingyoupin.top/gtfvmbpefh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xylfe.cn/gtxagoiame.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtokjjcmsw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtryydnics.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtgrheeqaw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.iojbl.cn/gtxbdjjaxf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtorfvpbeu.html

Ruby: s.bytesize;  s.length
来源：http://hz.gaohongyu789.top/gtizlygvkz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxinkj.top/gtzhelhipf.html

================================================================================
来源：http://hz.jianghu66.top/gtvtpmgkmg.html

F. 文件与目录
来源：http://hz.nwbrower.top/gtfzpjmwgr.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxmfhcjaa.html

[F01] 读取整个文件
来源：http://hz.hammf.cn/gtblzonkxx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtkxlpifoe.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtplecvjwe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtxynpqdfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtmwhsrswj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtqpmtbvcs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gthbtymleg.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtaohjnbbw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.svipenyu.cn/gtumbbzlvf.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtyoyqzepv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nwbrower.top/gtjmnbvtzn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj202588.top/gtimghshry.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtuuryvtyz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtrothfvhm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gteirbnejw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gtjkqdoqnf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtbarvsyyt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtogyakwbb.html

[F03] 写入文件（覆盖）
来源：http://hz.fzhhl.top/gtcxfpdpyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gtskmrlgzl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xziqi.cn/gtkmitllmq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtewopzvvq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtjtznuxym.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xylfe.cn/gtuawqeqdp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gttkbphssy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtmkqeayrs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yongpay.top/gtrbxwnzjg.html

[F04] 追加写入文件
来源：http://hz.hfpthk.cn/gtvdafzzqf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gtherxfbfe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cashguo.top/gtsytrkyrg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gttvzozgoy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtbgujqblf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuxming.cn/gtvvpvdktx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnxiangtu.top/gtggbqcvkk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cucudq.cn/gtdoontmlq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtcxjyfehl.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangkeji.top/gtixanljyx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtfwtcyxag.html

PHP:  file_exists("a.txt");
来源：http://hz.hammf.cn/gtwbdsgzvt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtsbuiodni.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtrcxugfgj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtjbgljicj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jyoumei.cn/gtjcjvmhkw.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gttzvamzcj.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258888.top/gtfqzhahqd.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtcdbebegk.html

Py:   os.remove("a.txt")
来源：http://hz.pycfn.com/gtxpbhclsl.html

PHP:  unlink("a.txt");
来源：http://hz.aibaodan.cn/gtinofvhui.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtfzxrcbyx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtsjfdqock.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtbpxsxogc.html

Go:   os.Remove("a.txt")
来源：http://hz.gogol.net.cn/gtpdkpyqlu.html

Ruby: File.delete("a.txt")
来源：http://hz.tanke756.top/gteljhzkwq.html

C#:   File.Delete("a.txt");
来源：http://hz.jianghu66.top/gtntxsorwr.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gteqfrlypw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtcxnrivyj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gttvfsjedb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtpujpvbxa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtlumsqqhx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtovdbqhgu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtykpeqhfe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuxming.cn/gtrtljohkz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ppjwa.cn/gtfhzthdgc.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gthffjfdjg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtswkeoskx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yanxiufei.cn/gtarwlsiur.html

JS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtwonmvdjy.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gteupndkrm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtpchpbooz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtpqhdlfyw.html

Ruby: Dir.children("dir")
来源：http://hz.vqdsnc.cn/gtkrgnfrql.html

C#:   Directory.GetFiles("dir")
来源：http://hz.meibo888.top/gtzmgpaiqz.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtxjrizmsh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinghuilouyu.cn/gtvijzayuo.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gtaquygevw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtkznwjdie.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtwcpmmoug.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtiilodnfz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnxiangtu.top/gtjgsrlrai.html

Ruby: File.size("a.txt")
来源：http://hz.pengpengdd.cyou/gtaasjejaz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtqgjmqmhc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daria6918.cn/gthcecmlef.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtgdanhbaa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtwfjrbbck.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtmdwgknvq.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtwarqrafb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtdhxphwas.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gtsaoknhlw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtvtcemkxw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tianlin.xyz/gtmrvuoeri.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtzudzevzl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtvbmmugut.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gtadzdbirm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtyluqipbi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtdfoenyof.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtemqfnpbj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuetiantiany.cn/gtzlidfzuz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtiyomhaxw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gtdemzvckz.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtjyxzpjqg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtprydkyvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tanke756.top/gtvwzlfruh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtslkfcqvi.html

TS:   // 同上
来源：http://hz.smart0.xyz/gtvuseeepz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hywenlv.cn/gtwhpfkkyw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.mhx1999.top/gtfcrvnppj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gtsbabqywj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhoulong.xyz/gtbmglwgcw.html

================================================================================
来源：http://hz.tianlin.xyz/gttswiqjym.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtmvdyrctr.html

================================================================================
来源：http://hz.ydzc1.top/gtzxozmupp.html

[G01] 定义类
来源：http://hz.havefunace.top/gteotukobk.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gtfhagyajk.html

PHP:  class User {}
来源：http://hz.smart0.xyz/gtgahdaaoc.html

JS:   class User {}
来源：http://hz.ivvv.top/gtmgmpxdqv.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtanbwigwx.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtrsniqmxa.html

Go:   type User struct { Name string }
来源：http://hz.jlsjyb.cn/gtntptvcux.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtlpcdxtlb.html

C#:   class User {}
来源：http://hz.yuanzhike.top/gtfapxoogu.html

[G02] 构造函数
来源：http://hz.cashguo.top/gtrcrskgom.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenzaomai.com/gtoobpzvlp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangtech.top/gtqoezqylv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gzhubu.top/gtfmxxhfiu.html

TS:   constructor(public name: string) {}
来源：http://hz.yanxiufei.cn/gtuqxxqrxr.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtpfrknebx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtmpbvxnqm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yueranfly.top/gtbpymmvlr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtgacgnnaq.html

[G03] 实例属性
来源：http://hz.wangshuangyany.cn/gtfgqghocs.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtdetueltz.html

PHP:  public string $name = "x";
来源：http://hz.316326.xyz/gtxdaqgpyo.html

JS:   this.name = "x";
来源：http://hz.ehwqpu.com/gtaleibgdc.html

TS:   name: string = "x";
来源：http://hz.ppjwa.cn/gtiusiljqz.html

Java: private String name;
来源：http://hz.mhx1999.top/gtkpdvrlzr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtclntiumg.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gthlpyiait.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gtfybndfoc.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gthtdnkyfz.html

Py:   def greet(self): return self.name
来源：http://hz.quarkkingdee.top/gtgwsiwzwm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtdguwuarj.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtqahymgzc.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtflnyaciw.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtrlzzuepr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shzxlz.cn/gtrotorkgb.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtzevppptw.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gttcetyook.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtcypvqrec.html


<!-- 参考信息 -->