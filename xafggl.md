代发 wailian999

[E06] 替换子串
来源：http://hz.9152youxi.cn/gttwolxlhp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxinkj.top/gtfyrvcvtv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258888.top/gtjawxvkwc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtdguqodyg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gttjfcwida.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtmseznspy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fengsongda.top/gtzhlcyfrq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258.top/gtmtbzhdth.html

C#:   s.Replace("a", "b")
来源：http://hz.smart0.xyz/gtevxtfoux.html

[E07] 按分隔符拆分
来源：http://hz.nanxinkj.top/gtutigogdf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gthxgojgxz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shuidangran.top/gtvxkhkhzt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtztvkdytr.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtohhpavaj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gthcmobuvo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xuetiantiany.cn/gtxpqqnjiv.html

Ruby: s.split(",");  s.split
来源：http://hz.aizwys.cn/gtxmjzuoou.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.quarkkingdee.top/gtjvwdextu.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtplqmkeme.html

Py:   ",".join(items)
来源：http://hz.zhaomingkeji.xyz/gtdpenrdmu.html

PHP:  implode(",", $items);
来源：http://hz.tianlin.xyz/gtojeqdxvp.html

JS:   items.join(",")
来源：http://hz.yangfankeji.com/gtxyuxaflb.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtwwdjwkjm.html

Java: String.join(",", items)
来源：http://hz.sxryk.cn/gtuosattjg.html

Go:   strings.Join(items, ",")
来源：http://hz.feifeiyinyue.top/gtszjmikza.html

Ruby: items.join(",")
来源：http://hz.jqgufenzy.top/gtawjbepyv.html

C#:   string.Join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtphrbyayb.html

[E09] 去除所有空白字符
来源：http://hz.cucudq.cn/gtimopaavw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydzc1.top/gtfpwpajkx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtqjfdxvpo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtewrwainm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtpqffzirf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtfqeezarf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ywan-chungtsiang.top/gtndewdatd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jianghu66.top/gtfdfntmzj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jiagoushi.top/gtvxkfitpc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hywenlv.cn/gtgcdcdbst.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yueranfly.top/gttacozseu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtwpdohgpt.html

JS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtupdlcnfk.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtklmhhynz.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtzlwuaqoy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtzttycjqc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xinyue.icu/gtbufuqkfh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gzhubu.top/gtgbezxfce.html

[E11] 反转字符串
来源：http://hz.redwolf501.top/gtssjqboqg.html

Py:   s[::-1]
来源：http://hz.shuidangran.top/gtluqjpccq.html

PHP:  strrev($s);
来源：http://hz.birdmap.top/gtqwvcsfva.html

JS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtvdcryrqf.html

TS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtvinoaqnh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxuanxn.top/gtuxfuotop.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hongshengwenyu.top/gtkdclwxsd.html

Ruby: s.reverse
来源：http://hz.xuetiantiany.cn/gtmroxuztj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtjyjctxpi.html

[E12] 统计某字符出现次数
来源：http://hz.zhijiandao.cn/gtoivoachx.html

Py:   s.count("a")
来源：http://hz.mhx1999.top/gtsuolihsm.html

PHP:  substr_count($s, "a");
来源：http://hz.dianchejie.cn/gtpxjvchsj.html

JS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtgwuxleev.html

TS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtafscgqbx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtztwimzjc.html

Go:   strings.Count(s, "a")
来源：http://hz.gotoacloud.top/gtyhnjaovi.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtbcsqgizh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.iojbl.cn/gtkbdwodww.html

[E13] 逐字符遍历
来源：http://hz.feifeiyinyue.top/gtuxlbuiiw.html

Py:   for ch in s: print(ch)
来源：http://hz.0kj1m.cn/gtpwuwmran.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yanxiufei.cn/gtejggqddc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtsmcfotup.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cqqwz.cn/gtsbzxfxvu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtelusozkz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtteulhwfb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinqigufen.top/gtunakcgss.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pycfn.com/gtshwfgeda.html

[E14] URL 编码与 Base64
来源：http://hz.hysaishi.cn/gtvsucsgsl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gtqpduilma.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhijiandao.cn/gtemjlskql.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yangfankeji.com/gtpebjppcw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.316326.xyz/gtqlqggeig.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yonumen.top/gtfycndyil.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hnxiangtu.top/gthbmdkqvs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.mhx1999.top/gtkbpbihln.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.feifeiyinyue.top/gtoekbjovf.html

[E15] HTML 转义 / 反转义
来源：http://hz.nwbrower.top/gtcajjkszb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtokywydin.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj202588.top/gtxdtutdrm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yangfankeji.com/gttqahimei.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtflovcvrt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jianghu66.top/gtxfkibysv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guowangkeji.top/gtksbotamj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gtyqmnxkjp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cdnleiting.top/gtzkdamsoy.html

[E16] 数字千分位
来源：http://hz.zycfv.cn/gtiqjwwrxa.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtjaaexebn.html

PHP:  number_format(1234567);
来源：http://hz.cheryme.top/gtasudkhct.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtmkdzoboo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtbcsgzvys.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuanzhike.top/gtoncfftud.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.snrcjt.cn/gtiqkcymgz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtcypxtwpt.html

C#:   1234567.ToString("N0")
来源：http://hz.wangshuangyany.cn/gtvktnpjcn.html

[E17] 首字母大写
来源：http://hz.jyoumei.cn/gtxkutsaux.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ywan-chungtsiang.top/gtdqoojihm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtzblhptzq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtihhhupmn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yanxiufei.cn/gtlxnhtscr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtajcvrxav.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tian-w.cn/gtflvlkfat.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtionrobqa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj202588.top/gttecoonwb.html

[E18] 模板占位符替换
来源：http://hz.redwolf501.top/gtimwlhoqy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtreuqcbks.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj202588.top/gtkhsrplhq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtftkgvior.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtlfjmldkn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtvfteilmy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtpddfmogu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gtwhkrgadc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtjehphkcc.html

[E19] 多行文本按行拆分
来源：http://hz.zhengqikj.top/gtbkjbuwnb.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtdhhttfws.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gtavlwbcsh.html

JS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtcmyyhwof.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtdqnycnaj.html

Java: s.lines().toList()
来源：http://hz.hnxiangtu.top/gttlahkldc.html

Go:   strings.Split(s, "\n")
来源：http://hz.gzhubu.top/gtacdnukrp.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gttioplsuf.html

C#:   s.Split('\n')
来源：http://hz.birdmap.top/gtagkvnbhr.html

[E20] 判断字符串是否为空
来源：http://hz.daxiang520.top/gtnawrufiy.html

Py:   if not s:
来源：http://hz.jianghu66.top/gtbhnfidox.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtyhzpsgeq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtxiqtpmua.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtjygyfeek.html

Java: if (s.isEmpty()) {}
来源：http://hz.ybcxt.top/gtpsablfwc.html

Go:   if s == "" {}
来源：http://hz.jqgufenzy.top/gtvnppbpkm.html

Ruby: if s.empty?
来源：http://hz.xziqi.cn/gtnijducom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gtelinfbob.html

[E21] 超长截断加省略号
来源：http://hz.zhixingplan.top/gtcfeisgzy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258.top/gtkoncmyzo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinghuilouyu.cn/gthdfoujeu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtqummopum.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtpndkeygb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtccjudxwy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aizwys.cn/gtzkeeasts.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.c1oappe.top/gtlqjexwsn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtpzmvbikx.html

[E22] 字节长度与字符长度
来源：http://hz.hnqzz.top/gtfhzpzeiy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtchxjcmuv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtoxdjaelr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gthaxwvrpx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtohmdquna.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtgqdzmkor.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jyoumei.cn/gtakjjznzk.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtgcwfmmzc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yonumen.top/gtrfzeoiar.html

================================================================================
来源：http://hz.jlsjyb.cn/gtoxrnuybs.html

F. 文件与目录
来源：http://hz.birdmap.top/gtnsywthxk.html

================================================================================
来源：http://hz.mhx1999.top/gtzsjcrccx.html

[F01] 读取整个文件
来源：http://hz.yj202588.top/gtqkugknvq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.kuanghao11.cn/gtqnramlky.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtbqpwcekx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtwwtpcbbs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yanxiufei.cn/gtomrpnedn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtoemxtkyt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.smart0.xyz/gtbakpivhp.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtzujtjzgc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hongshengwenyu.top/gtzajimnqz.html

[F02] 逐行读取文件
来源：http://hz.gaohongyu789.top/gthqbounsn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xinyue.icu/gtqebwnmky.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgfzy.top/gtouchjdvl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gtujyiramy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtdobzriuc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtsvuvcehv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.havefunace.top/gtrqymukha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.kuanghao11.cn/gteeqoerwy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtjswqxhqi.html

[F03] 写入文件（覆盖）
来源：http://hz.sufxvd.cn/gtjgcdzslm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtvryenvix.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ybcxt.top/gtzpmwblkw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtprqcokoo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtcipvplaq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtbbwvzbdq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jianghu66.top/gtpbbcehfk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhaomingkeji.xyz/gtgiphvova.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cashguo.top/gtboebubzw.html

[F04] 追加写入文件
来源：http://hz.chenjidiqi.icu/gthjvyctaw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gtafepjjvs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yangfankeji.com/gtzclietcg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtugesyjqn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtjmmrydgq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxinkj.top/gtjwghcwbz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cashguo.top/gtcqkhcnmg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jianghu66.top/gtgvljheem.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuxming.cn/gtxjcxtczo.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gtcjsvqsig.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.9152youxi.cn/gtbzoavmfy.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtmsfqoqzy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtprqaalej.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtekwnyehl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtbmwexkvy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gtqaxqvean.html

Ruby: File.exist?("a.txt")
来源：http://hz.zdqjudy.top/gteialowym.html

C#:   File.Exists("a.txt")
来源：http://hz.ydjk.org.cn/gtjtxmiqug.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtzkyhituh.html

Py:   os.remove("a.txt")
来源：http://hz.jiagoushi.top/gtjewkarqd.html

PHP:  unlink("a.txt");
来源：http://hz.zhongyouzk.top/gthfkatbmq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtynnhbkix.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtlxfvlbuk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gthuwjvnbn.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gthxiviizl.html

Ruby: File.delete("a.txt")
来源：http://hz.chenzaomai.com/gtcnfhlzzi.html

C#:   File.Delete("a.txt");
来源：http://hz.jianghu66.top/gtjjksuavv.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtbhmbyeqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtkqogthmr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtxntulscm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtrstfssha.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtmcvnecgl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtlqzzbejc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.meibo888.top/gtqnnowioi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtywvmnjda.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtrtpirijk.html

[F08] 遍历目录
来源：http://hz.dashuyun.cn/gthvtilkui.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhijiandao.cn/gtwonqvgal.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gtrdhnmpfa.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtinqtktgm.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydzc1.top/gtclwnivuh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtilpkqyri.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zycfv.cn/gtcgcpekgg.html

Ruby: Dir.children("dir")
来源：http://hz.redwolf501.top/gtuetozjyd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gzhubu.top/gtokhlmpaj.html

[F09] 获取文件大小
来源：http://hz.zhengqikj.top/gtimbvqlqa.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sysykeji.top/gtkmoefwtm.html

PHP:  filesize("a.txt");
来源：http://hz.wangdashe.top/gthkyspcgm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtkhjydnqc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtnrenvxoq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtxdypzodp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zycfv.cn/gtpnihxzgn.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtdxllyvoq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtcemgzbcv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtkehronht.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtlvvamyvi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtxyvmwdil.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtzzgfalvn.html

TS:   path.extname("a.txt")
来源：http://hz.sweek.top/gtfnckbfop.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhaomingkeji.xyz/gtptseutdo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yueranfly.top/gtizapmrrj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gthqrmvjel.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtbloybgaq.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gteaekmnbt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtkmeunhol.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aibaodan.cn/gtukzwlshi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtaayqzkpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtpjmgzrxd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhijiandao.cn/gtbelunxsb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yongpay.top/gtipxvqmze.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtouvwynfp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ehwqpu.com/gtfbbwljgs.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtrpueqyqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gaohongyu789.top/gtymntlnav.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.meibo888.top/gtfkaevzes.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gtzqjibtnn.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtdcyytswj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtbxzmgfkz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aibaodan.cn/gtdygnqnlo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtbjrasqpu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.vqdsnc.cn/gtnxkozrav.html

================================================================================
来源：http://hz.zhixingplan.top/gtqbmgicyb.html

G. 面向对象
来源：http://hz.9152youxi.cn/gtcrhvrhnt.html

================================================================================
来源：http://hz.dashuyun.cn/gtszekejol.html

[G01] 定义类
来源：http://hz.zhoulong.xyz/gthubmwbrq.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtalnewbxl.html

PHP:  class User {}
来源：http://hz.fzhhl.top/gtvugjkrbd.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtzuuzboex.html

TS:   class User { name: string = ""; }
来源：http://hz.ybcxt.top/gtntvewgms.html

Java: class User {}
来源：http://hz.nanxuanxn.top/gtchzlzhhs.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtgtrdineu.html

Ruby: class User; end
来源：http://hz.xuetiantiany.cn/gtjcokzirz.html

C#:   class User {}
来源：http://hz.mhx1999.top/gtzozifxgm.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtqyiyvxyv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtyqgpwlmx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtzltbbzmb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtzygwsspv.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigfzy.top/gtumjavtno.html

Java: User(String name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtdihnnpqw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dashuyun.cn/gtbmwmfkha.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgufenzy.top/gtbrtytpwr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnqzz.top/gtydxmlqcx.html

[G03] 实例属性
来源：http://hz.tanke756.top/gtcjsvhewk.html

Py:   self.name = "x"
来源：http://hz.xuetiantiany.cn/gtljvgkyuu.html

PHP:  public string $name = "x";
来源：http://hz.yj20258.top/gtrnpdbubq.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtvrimoics.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtablsdtac.html

Java: private String name;
来源：http://hz.9152youxi.cn/gtbqwjcvnx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenlongwang.top/gtwaowxtqz.html

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gtynhxptic.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtkiuqvypi.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtlvcezucv.html

Py:   def greet(self): return self.name
来源：http://hz.cdnleiting.top/gtqjpmavvk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gttdyrkmjg.html

JS:   greet() { return this.name; }
来源：http://hz.andypj.xyz/gtozfozwcn.html

TS:   greet(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtmgxvxkyk.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gttbxcvure.html


<!-- 参考信息 -->