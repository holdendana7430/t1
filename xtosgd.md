代发 wailian999

[E06] 替换子串
来源：http://hz.zycfv.cn/gthkitdqrp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.havefunace.top/gtihmukaoo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cdnleiting.top/gtczgfxypf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtgaeujcfj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtytpucrho.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtxidbzuqj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.snrcjt.cn/gtxgxmpegb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuanzhike.top/gtdwhlgend.html

C#:   s.Replace("a", "b")
来源：http://hz.xziqi.cn/gtredwfkqg.html

[E07] 按分隔符拆分
来源：http://hz.birdmap.top/gtknqdaepw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gtlxatszbw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gtliiqwbmh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuxming.cn/gtrztxoxna.html

TS:   s.split(",")
来源：http://hz.ydzc1.top/gthptpxzmw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gogol.net.cn/gtdonxgfoz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cheryme.top/gtuuyiilza.html

Ruby: s.split(",");  s.split
来源：http://hz.yongpay.top/gtkuvenmmh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gtcixlryty.html

[E08] 数组按分隔符合并
来源：http://hz.ivvv.top/gtkpzovxqg.html

Py:   ",".join(items)
来源：http://hz.sysykeji.top/gtjfbbojha.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtzlyshjam.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtakwbzjqw.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtvqmdfyly.html

Java: String.join(",", items)
来源：http://hz.zhixingplan.top/gtghhemoww.html

Go:   strings.Join(items, ",")
来源：http://hz.chenjidiqi.icu/gtaalquven.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtlobdvhmd.html

C#:   string.Join(",", items)
来源：http://hz.hysaishi.cn/gttqxolmel.html

[E09] 去除所有空白字符
来源：http://hz.zhijiandao.cn/gtfffrsgli.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hongshengwenyu.top/gtszovwzxt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aizwys.cn/gtauwpcdea.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gtnwndhmum.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtvnzapuzs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gttugnaitq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.mhx1999.top/gtrfpfrctt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gtomsnrclm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gotoacloud.top/gtfqefawis.html

[E10] 左侧补零 / 定长填充
来源：http://hz.bjfxy.top/gtjhtzatis.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gtavwulmpx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dashuyun.cn/gtwcttfegu.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtncjkmfvc.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtgvilnyrw.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtvmsrzown.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258888.top/gtfglgeydb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtxpvmbalx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jyoumei.cn/gtpkthrutl.html

[E11] 反转字符串
来源：http://hz.birdmap.top/gtzdwjlcjq.html

Py:   s[::-1]
来源：http://hz.jqgfzy.top/gtioknmccs.html

PHP:  strrev($s);
来源：http://hz.quarkkingdee.top/gtuxrhxkgh.html

JS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtcghgtmeg.html

TS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtltkrcida.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zycfv.cn/gtilzweyea.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gtrpjlpkzs.html

Ruby: s.reverse
来源：http://hz.jyoumei.cn/gtjntmhnhw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtlfjjvllr.html

[E12] 统计某字符出现次数
来源：http://hz.zhixingplan.top/gtshtipcww.html

Py:   s.count("a")
来源：http://hz.ydzc1.top/gtlafbhfbc.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gtplmijsbe.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtpakpdubx.html

TS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtoonnjpuo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xylfe.cn/gtwpucixco.html

Go:   strings.Count(s, "a")
来源：http://hz.zhiwuduotai.top/gtkbgtmkns.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtandlpkdk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ppjwa.cn/gtftacibew.html

[E13] 逐字符遍历
来源：http://hz.9152youxi.cn/gtnaoowiza.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxuanxn.top/gtoowxrmfy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aibaodan.cn/gtepezygel.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtxkvyksoo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtmbmcmoyy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigfzy.top/gtuqnwxftb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.haohaochexian.top/gtmxxfbvmc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtxzwxekau.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtgpxpjiuk.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangkeji.top/gtkfaxysne.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtwplmexqv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aibaodan.cn/gtsbhzggyr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtevrnwzuc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gthscjuaja.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gteesaufjc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtsfqgbqyp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.kuanghao11.cn/gttyuxlxcm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tianlin.xyz/gtmxgievhl.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhijiandao.cn/gtuhvbujsn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtszwlkesr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtbohztpol.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydjk.org.cn/gtjxrywzfq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sufxvd.cn/gtqhqnbpqz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258.top/gtjsgfpgos.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jiagoushi.top/gtmktwpmvt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jyoumei.cn/gtsjdattao.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtamtnbhzo.html

[E16] 数字千分位
来源：http://hz.pycfn.com/gtaexklnzb.html

Py:   f"{1234567:,}"
来源：http://hz.aibaodan.cn/gtpsrqgnlg.html

PHP:  number_format(1234567);
来源：http://hz.hfpthk.cn/gtjeljvycp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gthmlplvkk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtcwfgslfd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtcugpziam.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.havefunace.top/gtoznugqre.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgufenzy.top/gtxqbxdsvs.html

C#:   1234567.ToString("N0")
来源：http://hz.feifeiyinyue.top/gtycyxmxxe.html

[E17] 首字母大写
来源：http://hz.yj202588.top/gtiujjyjsl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gzhubu.top/gtimmknnii.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.bjfxy.top/gtwagnxmph.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtiyhnkbaa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtvdeprsit.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhongyouzk.top/gtgzuysfaa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jlsjyb.cn/gtrwbughol.html

Ruby: s.capitalize
来源：http://hz.yueranfly.top/gtuesjwrmi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hfpthk.cn/gtyejmqshi.html

[E18] 模板占位符替换
来源：http://hz.tian-w.cn/gtrvhejdfp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtvuuznbep.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtigezukav.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtbrcbyjzh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtxrgyrajc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shzxlz.cn/gtgfyikipm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenjidiqi.icu/gtkbyuxnbb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xziqi.cn/gtpyzwfclw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgufenzy.top/gtmphuziad.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtlkbvfnpn.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtehseofat.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gtmgayyscd.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtirlwxtdg.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtpcuquhkd.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtnunjeqrr.html

Go:   strings.Split(s, "\n")
来源：http://hz.tanke756.top/gtalmcvapz.html

Ruby: s.lines
来源：http://hz.chenjidiqi.icu/gtaqzmlukr.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtpjvgyffn.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gtedklesbc.html

Py:   if not s:
来源：http://hz.havefunace.top/gttsshgvac.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.wangshuangyany.cn/gtqoqgbacd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtsfwkoiab.html

TS:   if (s === "") {}
来源：http://hz.daria6918.cn/gtxczohsnq.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtajdramff.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtbamyvrxn.html

Ruby: if s.empty?
来源：http://hz.jyoumei.cn/gtuubjkgbb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtgttjligi.html

[E21] 超长截断加省略号
来源：http://hz.zdqjudy.top/gttkkagere.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nwbrower.top/gtpvfpflgu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sysykeji.top/gtkhnxyphl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtpjsysirp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtjwuliqab.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtpmddsfbg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zycfv.cn/gtuwqsebmk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hywenlv.cn/gtboiabwlf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cheryme.top/gtzivzcris.html

[E22] 字节长度与字符长度
来源：http://hz.vqdsnc.cn/gtkdsopskn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtxciyrerb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtfvqhtjzo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtaourfnhi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtzfemmrsp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtozjrhisd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ydjk.org.cn/gtoqoucnia.html

Ruby: s.bytesize;  s.length
来源：http://hz.guowangkeji.top/gtvxfgceew.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.birdmap.top/gtvfaswhry.html

================================================================================
来源：http://hz.dashuyun.cn/gtvvzkgrhp.html

F. 文件与目录
来源：http://hz.xuanzx.com/gttokshauu.html

================================================================================
来源：http://hz.dianchejie.cn/gtqukuknny.html

[F01] 读取整个文件
来源：http://hz.zycfv.cn/gtjcquwdsl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gticnegzxo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtkbzfykvn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhijiandao.cn/gtmmrcrkxl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ivvv.top/gtklbnlzaq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtlgicnesk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yonumen.top/gtlyxnpvnp.html

Ruby: File.read("a.txt")
来源：http://hz.jyoumei.cn/gtkvgfijja.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinghuilouyu.cn/gtpgkxfarl.html

[F02] 逐行读取文件
来源：http://hz.andypj.xyz/gtqncnflcu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtikqsmzxy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.meibo888.top/gtdmoymowh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtmtyeltwe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtoxftxmah.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtqudrmmkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtmnouhopn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.iojbl.cn/gtfylwnetc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.c1oappe.top/gtzqbfptxn.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtyylyuiii.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtanarzwfk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtshvbxuzr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtroijxags.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtxhchrxlr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangshuangyany.cn/gtmjqcixkh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daxiang520.top/gtyyprgykq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtpxzipvvk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cashguo.top/gtlbcdpikn.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gtzhkgkntl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gtgosgqxvr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtxlmtpyzk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtyiiarcne.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gttdvyycvq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtnnojyclm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtpwapmqid.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinghuilouyu.cn/gtazuvkzuj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtshfndnkh.html

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtnfaydxau.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fzhhl.top/gtqnvjdask.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtneiftrvz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtcxpocwht.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtcdpzntgt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtovtgwcfg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtrcdbthyn.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtuebjwctr.html

C#:   File.Exists("a.txt")
来源：http://hz.meibo888.top/gtnqczqcsc.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtxwwhaoic.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gteppdmflh.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258.top/gtdsodnwou.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtsbltingr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtyenlmuhc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtnzecwdrf.html

Go:   os.Remove("a.txt")
来源：http://hz.redwolf501.top/gtzoclyzzo.html

Ruby: File.delete("a.txt")
来源：http://hz.yanxiufei.cn/gtzrehylmr.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gtduysibmt.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtyldytwyb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigfzy.top/gtvuayrmkg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgufenzy.top/gthjztetzn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtwcxsouwp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtvfstseau.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258.top/gtidmcgwmx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtpyelznfo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.haohaochexian.top/gtjeamijbu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.haohaochexian.top/gtdjanctpy.html

[F08] 遍历目录
来源：http://hz.yj20258888.top/gtxqnnzmok.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtjkbqlqyo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hongshengwenyu.top/gtzgbwtnmw.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtiagymhqt.html

TS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtisrmzkqs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtituroone.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jyoumei.cn/gtojcwiebw.html

Ruby: Dir.children("dir")
来源：http://hz.zhaomingkeji.xyz/gtvmoxlwev.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtszwwrerd.html

[F09] 获取文件大小
来源：http://hz.jinqigufen.top/gtzmajvprz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gttbvtuugv.html

PHP:  filesize("a.txt");
来源：http://hz.vqdsnc.cn/gtcoxwzyev.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtqgrxcdkj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtbbpsyvdm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtmwughggu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258.top/gtsysvtfcy.html

Ruby: File.size("a.txt")
来源：http://hz.cdnleiting.top/gtkzdcejbg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yanxiufei.cn/gtulbvvgid.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jyoumei.cn/gtkqeprvgm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtgztrdnve.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj202588.top/gtbvgkjwpd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtvkptykoi.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gttmtbdmdr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.birdmap.top/gtdhqnucbx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gtvjpckkfk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtdkhsxtcv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtgksvtcsa.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gtsubgfvjr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtxcgtvhad.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtxlapocnk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtlojbonyu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtmjgtcnvz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gtmimyomlo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gotoacloud.top/gtcvgnpokn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtcqfkjpnb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gttdwgujrk.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtzqesuzjz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nwbrower.top/gteyppzgvw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gthofzcpzh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtfnmrqgca.html

TS:   // 同上
来源：http://hz.birdmap.top/gtrwyjzkkj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtgapoxjfv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtzlvkxqcs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aibaodan.cn/gtcsavkihv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gtfawodhlw.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfxqqcbdq.html

G. 面向对象
来源：http://hz.meibo888.top/gtexizsnwi.html

================================================================================
来源：http://hz.zhongyouzk.top/gtdqbuwszi.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtermxshch.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtkvjtnykp.html

PHP:  class User {}
来源：http://hz.shuidangran.top/gthejeojpo.html

JS:   class User {}
来源：http://hz.cucudq.cn/gtdnsqzpaz.html

TS:   class User { name: string = ""; }
来源：http://hz.ywan-chungtsiang.top/gtlkgnzihb.html

Java: class User {}
来源：http://hz.hysaishi.cn/gtorsxsjfr.html

Go:   type User struct { Name string }
来源：http://hz.yvedp.cn/gtbsfrtazt.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtyfcymgcf.html

C#:   class User {}
来源：http://hz.yj20258888.top/gtskpvmbfa.html

[G02] 构造函数
来源：http://hz.zhiwuduotai.top/gtbbyuncbh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pycfn.com/gtxeglqpox.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhaomingkeji.xyz/gtnwqvhfdc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtlpronxhl.html

TS:   constructor(public name: string) {}
来源：http://hz.52xcode.cn/gtwevjbgtt.html

Java: User(String name) { this.name = name; }
来源：http://hz.tian-w.cn/gtwiyzsuyt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtiwlnormk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtptqbbduf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtpsvekvaz.html

[G03] 实例属性
来源：http://hz.daria6918.cn/gtkhmavcjq.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtpjvrsjpk.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtqtkbtjjz.html

JS:   this.name = "x";
来源：http://hz.xuanzx.com/gtykrmntzp.html

TS:   name: string = "x";
来源：http://hz.ydjk.org.cn/gtemsmxlnj.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtgrpwjubi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pycfn.com/gtamtmsipn.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtraagaidm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gtyprgyfjb.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtovrpaijt.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtsszgueem.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtdfkjppkv.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtsfdjaqzv.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gtmeqomkjr.html

Java: String greet() { return name; }
来源：http://hz.c1oappe.top/gtxukjzpjc.html


<!-- 参考信息 -->