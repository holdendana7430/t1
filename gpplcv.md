代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangkeji.top/gtsnhmdswx.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gtexvfkhgf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258.top/gtywhpqnxf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hfpthk.cn/gtcpqheefn.html

Ruby: s.split(",");  s.split
来源：http://hz.snrcjt.cn/gtdcgjsfio.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shanyushiyangtech.top/gtmeksahis.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtmwomgdui.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gthdmerfoi.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtmfpemqfx.html

JS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtpnqfwtno.html

TS:   items.join(",")
来源：http://hz.cucudq.cn/gtymwzcadx.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtwdhvxyto.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gtourkfnmg.html

Ruby: items.join(",")
来源：http://hz.andypj.xyz/gtglyjpbor.html

C#:   string.Join(",", items)
来源：http://hz.52xcode.cn/gtcifggtdw.html

[E09] 去除所有空白字符
来源：http://hz.snrcjt.cn/gtqiewzvgm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jlsjyb.cn/gtnewvtftp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtabkzdngs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtnnnyoyjt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtwehyhdpf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtnrsjpwwn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aizwys.cn/gtairknexj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sxryk.cn/gtzqpqoqev.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gthlhnzeqv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ehwqpu.com/gtddnomsxe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtubncdtxb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhaomingkeji.xyz/gtcnqnimun.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtbnglxuwl.html

TS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gthvrsayny.html

Java: String.format("%03d", 7)
来源：http://hz.gogol.net.cn/gteojarhbz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gtwafbaczi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gtayicgubv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yueranfly.top/gtvnzjcuxb.html

[E11] 反转字符串
来源：http://hz.xuanzx.com/gtyqioilkl.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtmjbipjid.html

PHP:  strrev($s);
来源：http://hz.tanke756.top/gtsfwwidiy.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtzyzglhon.html

TS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtyyovjzsa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aibaodan.cn/gtintkxghv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydjk.org.cn/gtonwfmvjl.html

Ruby: s.reverse
来源：http://hz.hammf.cn/gtfobkyawy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gttpysurqn.html

[E12] 统计某字符出现次数
来源：http://hz.xuanzx.com/gtxuvheokh.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gteckxkxaf.html

PHP:  substr_count($s, "a");
来源：http://hz.xuanzx.com/gtdfnmqaiw.html

JS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gthrfdfens.html

TS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtyqrwzcns.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.andypj.xyz/gtqqvrozsy.html

Go:   strings.Count(s, "a")
来源：http://hz.shzxlz.cn/gtiwcxhwps.html

Ruby: s.count("a")
来源：http://hz.cheryme.top/gtfyfekjqh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gteotlknfd.html

[E13] 逐字符遍历
来源：http://hz.shzxlz.cn/gtpqcsisbt.html

Py:   for ch in s: print(ch)
来源：http://hz.snrcjt.cn/gtvjlnzovf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtrnrnocxe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtcweyxuro.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtqwuwbykj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zdqjudy.top/gtillxmlfx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shuidangran.top/gtbohclhdb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtddxtjmec.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dashuyun.cn/gtvhwwzyjj.html

[E14] URL 编码与 Base64
来源：http://hz.hywenlv.cn/gtiriyeefh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydjk.org.cn/gtqsowaelf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.havefunace.top/gtpdxnyorh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gthtatoazc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gtrjlfapcx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.c1oappe.top/gtljfpcvsv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.iojbl.cn/gtdzavsylj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yangfankeji.com/gtnbaqitjy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yonumen.top/gtyyzrbtud.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtxpjhdpay.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ybcxt.top/gtgcibatla.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guowangkeji.top/gtjpwadvpo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.andypj.xyz/gtgekodoup.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yongpay.top/gtlkbzlixp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.snrcjt.cn/gtxyajtvcl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gtfugdqjqu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigufen.top/gtxsmtqpaa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.316326.xyz/gtyctdbefv.html

[E16] 数字千分位
来源：http://hz.xinyue.icu/gtmufleevz.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigufen.top/gtnfnlqxhq.html

PHP:  number_format(1234567);
来源：http://hz.wangdashe.top/gtcyyiwkme.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtdhumfwvy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtwfpmhxij.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gtnufsjzjn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtrreoxqtu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hfpthk.cn/gtifenbsan.html

C#:   1234567.ToString("N0")
来源：http://hz.sxryk.cn/gtgqtmukvn.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtamnebtnv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxuanxn.top/gtzotvxzfk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangshuangyany.cn/gtjlkqisqr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gthckhuafp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtdelgbnnp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pengpengdd.cyou/gtwairyebw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sysykeji.top/gtoijngghi.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtfxbdnopq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xingfuxueyuan.xyz/gtjbqwwcfk.html

[E18] 模板占位符替换
来源：http://hz.jinqigufen.top/gtvpfqtlgy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtwtehlxoy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydzc1.top/gtedkghaql.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtyctczkqy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtaepptdvr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yanxiufei.cn/gtcpwdpunn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtbvxdirji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhoulong.xyz/gtkspqgare.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pycfn.com/gtwnczotkd.html

[E19] 多行文本按行拆分
来源：http://hz.zdqjudy.top/gtyzuwewpu.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gttanxidom.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dashuyun.cn/gtlfrdrxzt.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtklzphpbr.html

TS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtgwprmght.html

Java: s.lines().toList()
来源：http://hz.zhengqikj.top/gtpwiqhery.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtvmlqfmdb.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gtiliuwjje.html

C#:   s.Split('\n')
来源：http://hz.birdmap.top/gtbpasszvv.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtvjnuojob.html

Py:   if not s:
来源：http://hz.xylfe.cn/gtnbyiqokw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxinkj.top/gtsubmsvoi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cheryme.top/gtylfikils.html

TS:   if (s === "") {}
来源：http://hz.yonumen.top/gttkitcuyg.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtfroohlan.html

Go:   if s == "" {}
来源：http://hz.wangshuangyany.cn/gtvhxaotto.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtduchwbll.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.bjfxy.top/gtxtslvtvw.html

[E21] 超长截断加省略号
来源：http://hz.kuanghao11.cn/gttrpslhqk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtfkglrtii.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenlongwang.top/gtksvxixzn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtraosvuwd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtsurcjxeb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtgtjylrhp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fzhhl.top/gtkyhpfbzr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.birdmap.top/gtcxaywyea.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtoyyybrib.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtkfzsmkej.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pengpengdd.cyou/gtytzxcubt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtoweshlvn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtpzrgrzqs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtszdtvlpo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtowlslwmt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daxiang520.top/gtcrjnvhtc.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtrgbcvkdb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangdashe.top/gtzehbjsie.html

================================================================================
来源：http://hz.sxryk.cn/gtqlwkldyq.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gttjpmwlbz.html

================================================================================
来源：http://hz.gaohongyu789.top/gtdnrxssod.html

[F01] 读取整个文件
来源：http://hz.kuanghao11.cn/gtqiwvjfge.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtgwbhexct.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daxiang520.top/gtjuarfmkb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhixingplan.top/gtmrgsmthk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgufenzy.top/gtszrhnytq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gttbwpyemu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hfpthk.cn/gttcpxddmk.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gtmhusfaqe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtbenidspj.html

[F02] 逐行读取文件
来源：http://hz.redwolf501.top/gttpfcvnfl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dashuyun.cn/gtidkcqhpt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinghuilouyu.cn/gtszltpjhd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtsswvrpsw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtlkluqoef.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtfcgdnsgv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xingfuxueyuan.xyz/gtsrhgualm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.svipenyu.cn/gtlpzlshym.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtrgqwukko.html

[F03] 写入文件（覆盖）
来源：http://hz.snrcjt.cn/gtdrzvrrvl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.haohaochexian.top/gtshmvbbhq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jianghu66.top/gtjtcltvuq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gthijwqvwb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtbgquyvfe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigfzy.top/gtfheuyhtp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.haohaochexian.top/gtdiatyhwe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinyuanbaomall.cn/gtzvdunijp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtomuzixcl.html

[F04] 追加写入文件
来源：http://hz.sxryk.cn/gttsvlmzzq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jlsjyb.cn/gtmyxcrbxl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtvseuayky.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtmuezctja.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtwxleznbu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigfzy.top/gtmvezoabc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtcytiluhb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sxryk.cn/gticbykwlo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gtelvbqxab.html

[F05] 判断文件或目录是否存在
来源：http://hz.jlsjyb.cn/gtyvygntij.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.snrcjt.cn/gtbjmlrvbd.html

PHP:  file_exists("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtbmfqmjhb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gthmwqlutu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtlmszggyv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtogbahcsf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj202588.top/gtqjhzlsch.html

Ruby: File.exist?("a.txt")
来源：http://hz.gotoacloud.top/gtpcrwhqmq.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxuanxn.top/gtsdmbyxzr.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gtebygolqo.html

Py:   os.remove("a.txt")
来源：http://hz.jlsjyb.cn/gtaoyhjwmu.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtiqkzmhpr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jlsjyb.cn/gtqnbkidob.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gthkoqvlhp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtxxvlqcbs.html

Go:   os.Remove("a.txt")
来源：http://hz.yueranfly.top/gtrtnzaprt.html

Ruby: File.delete("a.txt")
来源：http://hz.daria6918.cn/gtjtskkxwc.html

C#:   File.Delete("a.txt");
来源：http://hz.cashguo.top/gtauubqztb.html

[F07] 创建目录（含多级）
来源：http://hz.cucudq.cn/gtipgurujc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gogol.net.cn/gtcnnhqfiy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtxoykvqwd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtfrgnsdeq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gtbmsfncuu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.mhx1999.top/gtckclkepa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtfwnqmmbl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gzhubu.top/gtkhgzflbx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtwoiyihew.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gticmkulxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtmvcftxwx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.52xcode.cn/gtssziqqsw.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtdficoqfm.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtacxztlvt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtpuoybhiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtyzgabkqk.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gthxrugqzq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shzxlz.cn/gtqdrnstyo.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtlkbnoxhy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tanke756.top/gtmqthoolr.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtjufoezty.html

JS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gttpvjasfa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtvrhgykxl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtxnmxfyie.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtjwwdqrwm.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtzbezulpb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangdashe.top/gtvmslhbjp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtkzcqcsid.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtvlyniqvj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhiwuduotai.top/gtahfxkkop.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtkarzwjrf.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtzjrtstbx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gtnyjfctoz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtmzzjlpsl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtavgzeohk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtzfwfrigf.html

[F11] 复制与移动文件
来源：http://hz.zhixingplan.top/gtjegppojh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtycjruuqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pengpengdd.cyou/gtxbigdjqr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtmtnbxctr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtcnmuceub.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhongyouzk.top/gtrysmkfcp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigufen.top/gtvzcueywa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtdlhdfvix.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangshuangyany.cn/gtmhsuazaa.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gtuujvkelf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtxsuogsqz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gtlnpcnjjg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daxiang520.top/gtlygeccny.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtfgwudadm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yonumen.top/gtmlzvnnzy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtauwulzge.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.haohaochexian.top/gtmyvjrdhd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yueranfly.top/gtgigdovgu.html

================================================================================
来源：http://hz.yj202588.top/gteqcockbb.html

G. 面向对象
来源：http://hz.xuetiantiany.cn/gtpobjoowx.html

================================================================================
来源：http://hz.daxiang520.top/gtgihmftzt.html

[G01] 定义类
来源：http://hz.aibaodan.cn/gtqkhqebee.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gtulcftmgm.html

PHP:  class User {}
来源：http://hz.c1oappe.top/gtoyrjshet.html

JS:   class User {}
来源：http://hz.yj20258888.top/gtebwoybqx.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtqzwyextk.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtteziscvo.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gtffasletc.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtiiyuxagv.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtayfcanlw.html

[G02] 构造函数
来源：http://hz.ydzc1.top/gtvymywguh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtgejlkohh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuanzx.com/gtaahbzxil.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtxirvedfb.html

TS:   constructor(public name: string) {}
来源：http://hz.xylfe.cn/gtwtpwvcku.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtapksilsb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtpdbctndm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtdozthdhz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtspyhtxia.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtrjwsalco.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtcxjymvaa.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtrnlsguju.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtxekpiydw.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gtyyxsfkxa.html

Java: private String name;
来源：http://hz.hongshengwenyu.top/gtyqdutgpo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenjidiqi.icu/gtxzkkoxla.html

Ruby: @name = "x"
来源：http://hz.c1oappe.top/gtuouvtepu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.redwolf501.top/gtrhptaayg.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtxivynrgb.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtrojxsrnv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtjopbxwih.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtrotvqikv.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtcxcwtexl.html

Java: String greet() { return name; }
来源：http://hz.zhoulong.xyz/gtfvgqotkp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.birdmap.top/gtbnmauhli.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtcxwowvkc.html

C#:   public string Greet() => Name;
来源：http://hz.fzhhl.top/gtwglkvdrf.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtmrdayupx.html

Py:   class Admin(User): pass
来源：http://hz.nanxinkj.top/gtzhwzotaq.html

PHP:  class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtunpmukhg.html

JS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtzvvozaym.html

TS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtqytqdtau.html

Java: class Admin extends User {}
来源：http://hz.jiagoushi.top/gtfxzeqksu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtcberhbht.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gticreqlgk.html

C#:   class Admin : User {}
来源：http://hz.jianghu66.top/gtcgsjojkt.html


<!-- 参考信息 -->