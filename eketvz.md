代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtdbjjwnqs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtzuwtumip.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuetiantiany.cn/gtawlazmly.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtilatqvuv.html

C#:   s.Replace("a", "b")
来源：http://hz.chenzaomai.com/gtwqlrfifg.html

[E07] 按分隔符拆分
来源：http://hz.gzhubu.top/gtgcbwhzvm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ivvv.top/gtibykejaf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gtbsgonvwu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sufxvd.cn/gtapoyhdns.html

TS:   s.split(",")
来源：http://hz.ydjk.org.cn/gtgcmnijft.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhaomingkeji.xyz/gtxidhedxq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zdqjudy.top/gtznbhqqdi.html

Ruby: s.split(",");  s.split
来源：http://hz.tanke756.top/gtnjhacono.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zdqjudy.top/gtkifhhclp.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtuojkcmkk.html

Py:   ",".join(items)
来源：http://hz.gaohongyu789.top/gthmzdpiar.html

PHP:  implode(",", $items);
来源：http://hz.yvedp.cn/gtesrqzzrs.html

JS:   items.join(",")
来源：http://hz.ehwqpu.com/gtclpavqkh.html

TS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtzcetioak.html

Java: String.join(",", items)
来源：http://hz.zhijiandao.cn/gtpmsgrbwg.html

Go:   strings.Join(items, ",")
来源：http://hz.xylfe.cn/gtrfcswrpl.html

Ruby: items.join(",")
来源：http://hz.cheryme.top/gtvvfpawpn.html

C#:   string.Join(",", items)
来源：http://hz.chenjidiqi.icu/gtzabuviug.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtiibtmbvl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cucudq.cn/gthpjnparu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtregfkngx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dianchejie.cn/gtbquloazm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtnyylrawn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.svipenyu.cn/gtpjqpimhr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guannengcc.top/gtgrzsxsgl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gtgnocvglj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtebsnywly.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yueranfly.top/gtppuydzjo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxinkj.top/gtbnlhbffm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gtdogwjgug.html

JS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtdheekfue.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtebjrkssc.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtydaahauj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnqzz.top/gtzusgxwgh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jiagoushi.top/gtomxsvsat.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.meibo888.top/gtdldungkt.html

[E11] 反转字符串
来源：http://hz.jinyuanbaomall.cn/gtohqakadn.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtmdkooopx.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtcjwwnnwj.html

JS:   [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtifaejuom.html

TS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtjroyfexi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydjk.org.cn/gtkzjknvle.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shuidangran.top/gttexxncby.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gtrzhshdmj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtxyqqjqsz.html

[E12] 统计某字符出现次数
来源：http://hz.svipenyu.cn/gtycfzapmw.html

Py:   s.count("a")
来源：http://hz.ydzc1.top/gttsyeruev.html

PHP:  substr_count($s, "a");
来源：http://hz.zhongyouzk.top/gtpvrwftnj.html

JS:   s.split("a").length - 1
来源：http://hz.meibo888.top/gtdnzpglvb.html

TS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtuonbvdil.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aizwys.cn/gtsfnytjht.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgfzy.top/gtlovtadbd.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtwakoikfx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtbdgsueam.html

[E13] 逐字符遍历
来源：http://hz.vqdsnc.cn/gtbimpngfl.html

Py:   for ch in s: print(ch)
来源：http://hz.yuxming.cn/gtlbeouxqj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenjidiqi.icu/gtbzennhvl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gtouwboexh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtqqaawtcg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ivvv.top/gtylcnvhjm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuanzx.com/gtnfnodkze.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtqghoclzf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yvedp.cn/gtjbujdhgl.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtzwzoiuws.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zdqjudy.top/gtajzgainq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pengpengdd.cyou/gtijovqpof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gtgaozybpy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dianchejie.cn/gtrhkxsgnu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guowangkeji.top/gtlgcxywip.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xziqi.cn/gtbndhscaz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ybcxt.top/gtkqodioaj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtbphixoob.html

[E15] HTML 转义 / 反转义
来源：http://hz.mhx1999.top/gtteazjtfq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ybcxt.top/gttuurunao.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gtawmjiazl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.0kj1m.cn/gtrdjxfelj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.vqdsnc.cn/gtymsbiyjq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnqzz.top/gthcejhuek.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gtsqppnogi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenjidiqi.icu/gtgfcnxqlx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtjcpljkwq.html

[E16] 数字千分位
来源：http://hz.nanxinkj.top/gtczdirgmy.html

Py:   f"{1234567:,}"
来源：http://hz.chenlongwang.top/gtrkklcqbu.html

PHP:  number_format(1234567);
来源：http://hz.zhiwuduotai.top/gtcrzmslil.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtntyibuof.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zdqjudy.top/gtdkhwkwya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtekrbfzhb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtjkqqhjqd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gotoacloud.top/gtjajhqbtp.html

C#:   1234567.ToString("N0")
来源：http://hz.hysaishi.cn/gttxjhopwf.html

[E17] 首字母大写
来源：http://hz.guowangkeji.top/gtcgcivvwg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.daria6918.cn/gtaxognmsy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtzcqcmqcs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtwpileztp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtqskwicrp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ehwqpu.com/gtpdxauxvv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gttwbjgfnl.html

Ruby: s.capitalize
来源：http://hz.shuidangran.top/gtacwjsngd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gtufeuqhbx.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gtzmnwsthb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtwlroryjv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtndmruqvs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtqzalixoz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtlomzltzi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sufxvd.cn/gtnlbxtbbg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pycfn.com/gtedcqqijp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258.top/gtigzwxife.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtivnkubkm.html

[E19] 多行文本按行拆分
来源：http://hz.ydzc1.top/gtyfubqsju.html

Py:   s.splitlines()
来源：http://hz.cheryme.top/gtpwxnzbde.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtdwbmxfqz.html

JS:   s.split(/\r?\n/)
来源：http://hz.gzhubu.top/gtyityaawi.html

TS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtjkwehjdd.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtqnupmtxi.html

Go:   strings.Split(s, "\n")
来源：http://hz.smart0.xyz/gtlnvpolut.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gtbgohzown.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtgvibsafy.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtrcbxnsfi.html

Py:   if not s:
来源：http://hz.hongshengwenyu.top/gtsesfbqar.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gtcwwtguyq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ivvv.top/gtmrbsmnuq.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gtblfvugmn.html

Java: if (s.isEmpty()) {}
来源：http://hz.yueranfly.top/gtfnnqtgmv.html

Go:   if s == "" {}
来源：http://hz.zhoulong.xyz/gtmoqrfhuq.html

Ruby: if s.empty?
来源：http://hz.cucudq.cn/gtvwthhwza.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jianghu66.top/gtwwlesfqe.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gtqtvugddz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtybrdgbge.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gttjdwlrzc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtcazlifuy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtspoddtyq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtdpidgplh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zdqjudy.top/gttbeszdwy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yonumen.top/gtjfvgykmt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtziokitkz.html

[E22] 字节长度与字符长度
来源：http://hz.yongpay.top/gtboihjpab.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tianlin.xyz/gtaldbicpy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtwvcbrlgi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtdhcdhzzt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtflevrsfm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cdnleiting.top/gtftrpddwl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dianchejie.cn/gthplqkdeu.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangshuangyany.cn/gtxnykamca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gttlupcfmn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjvgptxtd.html

F. 文件与目录
来源：http://hz.fengsongda.top/gttabswnzl.html

================================================================================
来源：http://hz.yonumen.top/gtonjpvndz.html

[F01] 读取整个文件
来源：http://hz.guannengcc.top/gtkzfikrda.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtbasesapm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jqgufenzy.top/gtdjufptxd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtiuwvhzvm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtyhurlaiz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtyjmpnbvf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yonumen.top/gtqnywmydr.html

Ruby: File.read("a.txt")
来源：http://hz.9152youxi.cn/gtoqhsuoyv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.quarkkingdee.top/gtaniazwip.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtrcorquxt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ybcxt.top/gtyufrsbok.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gogol.net.cn/gtrnyvhmak.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtoxnrswsk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gtawdofrkt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtypancvjc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gaohongyu789.top/gtwdwsmjim.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtjcxczstu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.svipenyu.cn/gtzjowdcwx.html

[F03] 写入文件（覆盖）
来源：http://hz.tian-w.cn/gttjhbmoku.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258888.top/gtdkorshzd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtxriavxik.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtsejembaq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gthsnhqyan.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gtclkwyjmy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258.top/gtivgvqmva.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hammf.cn/gtcvmvycqh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtmujybtxh.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtadjccbiz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtiubuthli.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtlwvcytwg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtvigsxqli.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtplvovfqm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daxiang520.top/gtwsshrbkn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtrentmloa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigufen.top/gthymxamfd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gtrhtfnzzg.html

[F05] 判断文件或目录是否存在
来源：http://hz.hammf.cn/gtqzhwkiqt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtlamppcjk.html

PHP:  file_exists("a.txt");
来源：http://hz.tian-w.cn/gtlxxywywv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtbiejnsjq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtzbxwezxj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtdxdmnegq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.birdmap.top/gtwcczpikj.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtyrhapahw.html

C#:   File.Exists("a.txt")
来源：http://hz.zhijiandao.cn/gtheflvsha.html

[F06] 删除文件
来源：http://hz.mhx1999.top/gtxoujsfku.html

Py:   os.remove("a.txt")
来源：http://hz.zhixingplan.top/gtzzqxjyzc.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtpdrbnejf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtbsyziohb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtgohltedx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtacjufrjp.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gtxtxkghcb.html

Ruby: File.delete("a.txt")
来源：http://hz.daria6918.cn/gtyjfsekso.html

C#:   File.Delete("a.txt");
来源：http://hz.gzhubu.top/gtetnzlpvz.html

[F07] 创建目录（含多级）
来源：http://hz.yvedp.cn/gtpnypetnk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.havefunace.top/gtzzlvwrnv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtztughztb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtrajigert.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtapcawwuj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtylkzddmw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtgashthhx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zycfv.cn/gtirgxrdwz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zycfv.cn/gtogbetgpr.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtcrxmiukw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xziqi.cn/gtbjszmrhr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shuidangran.top/gtiinlqrby.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtckrtdwic.html

TS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtomchehay.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtwpcwoyos.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gttahuimao.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtdszfokpn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jyoumei.cn/gtuonchssc.html

[F09] 获取文件大小
来源：http://hz.shangyingyoupin.top/gtolqztxbx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtnvaoyodo.html

PHP:  filesize("a.txt");
来源：http://hz.ppjwa.cn/gtelixfscy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtuohesoir.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gtyyzdogfs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtadgdlgik.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zdqjudy.top/gtxtqfxiqs.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtewofjeaz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.birdmap.top/gtqpvjsikh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tianlin.xyz/gtcmtkotzz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtjtshzdab.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jlsjyb.cn/gtakzxeqgu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtxbptzfrn.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtdagxgxqa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sweek.top/gtuowdgpmf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gtkdhfrfpd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtwtphahbg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtlhmaytqo.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gttmzlnsyw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtcsaudltk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtszvdoilf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtxtibjdbu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtvrpitphg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gtgsqlrzrs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daxiang520.top/gtsdkallyn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtvntjhgom.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dashuyun.cn/gtppcjcwnp.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gteizoekhv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtbbzuhhvb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtciwtejuj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtuskhowir.html

TS:   // 同上
来源：http://hz.sweek.top/gtgqowfjkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xingfuxueyuan.xyz/gtsifntdka.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aizwys.cn/gtowybdwjj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtekirasml.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.mhx1999.top/gtfwhslcgy.html

================================================================================
来源：http://hz.jinqigufen.top/gtlofbedum.html

G. 面向对象
来源：http://hz.yvedp.cn/gtsxnzybty.html

================================================================================
来源：http://hz.cucudq.cn/gtzrkjeagt.html

[G01] 定义类
来源：http://hz.tanke756.top/gtkbzotczt.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtamgizuhe.html

PHP:  class User {}
来源：http://hz.cheryme.top/gtfwqaaxaw.html

JS:   class User {}
来源：http://hz.yangfankeji.com/gtpbtwazmr.html

TS:   class User { name: string = ""; }
来源：http://hz.yanxiufei.cn/gtzxcykqaz.html

Java: class User {}
来源：http://hz.fzhhl.top/gthqnoxryy.html

Go:   type User struct { Name string }
来源：http://hz.yuxming.cn/gtfyywrsck.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gtkzzhalou.html

C#:   class User {}
来源：http://hz.kuanghao11.cn/gturwpyyan.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gtijoygbgk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtioylabix.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinghuilouyu.cn/gtqdepgpdz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtjpsplzrq.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtkzcqsnyj.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtnnpagbzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gaohongyu789.top/gtwyabfryu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.0kj1m.cn/gtddiytizm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.kuanghao11.cn/gthukdrjps.html

[G03] 实例属性
来源：http://hz.yuanzhike.top/gtzbamuixx.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gtewrfphxo.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gttuuthkyk.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtlvdnygcx.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtqxrpbmvr.html

Java: private String name;
来源：http://hz.sweek.top/gtydbddbpu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhoulong.xyz/gtqtjtfsyf.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtxmrxdgkq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtspxnbhzg.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtdqbodtkn.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtcjsejwfq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtnqxzjvjo.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gtfsnmazdq.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtysmlpoqc.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtxteimyad.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtdhenepxu.html

Ruby: def greet; @name; end
来源：http://hz.hfpthk.cn/gtmfkrnfzw.html

C#:   public string Greet() => Name;
来源：http://hz.quarkkingdee.top/gtfncgpwqw.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtqoseyrxb.html


<!-- 参考信息 -->