代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.jqgfzy.top/gtixxpxeut.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tianlin.xyz/gtrgwtdhnr.html

[E08] 数组按分隔符合并
来源：http://hz.vqdsnc.cn/gtgzlrtjam.html

Py:   ",".join(items)
来源：http://hz.gzhubu.top/gtaxyzvlnw.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtyurkhuta.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtjplxdmnv.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtcmkankex.html

Java: String.join(",", items)
来源：http://hz.zdqjudy.top/gtszjjsdht.html

Go:   strings.Join(items, ",")
来源：http://hz.zhiwuduotai.top/gtybrtkanm.html

Ruby: items.join(",")
来源：http://hz.jinghuilouyu.cn/gtnftbckdn.html

C#:   string.Join(",", items)
来源：http://hz.ybcxt.top/gtvesxdkfg.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gtgplhcjup.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtiquphwae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gtvpfzsaov.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hnxiangtu.top/gtyjjewyhz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtogudotqt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ydjk.org.cn/gtrqdfohko.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.iojbl.cn/gtphjisvcz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtjdhyfkrm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangshuangyany.cn/gtlvytlrmr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.quarkkingdee.top/gtetwtfzee.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tanke756.top/gtswvfwcpf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fzhhl.top/gtjuvmbhce.html

JS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtizkgnjla.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtlejxgeci.html

Java: String.format("%03d", 7)
来源：http://hz.hysaishi.cn/gtiqtliwgm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tanke756.top/gtkumfhuhj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtnkxyszmt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigufen.top/gtrzgtqsrt.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtwuafwkoi.html

Py:   s[::-1]
来源：http://hz.vqdsnc.cn/gthyoinjfe.html

PHP:  strrev($s);
来源：http://hz.yj20258.top/gtorxgwvua.html

JS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtanhbzebs.html

TS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtleddtjdi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.mhx1999.top/gtztvytyqu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ywan-chungtsiang.top/gtcwbythzy.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gtmguezuvu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtexqlgnbg.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtqwzzkxex.html

Py:   s.count("a")
来源：http://hz.fzhhl.top/gtqvsndbwz.html

PHP:  substr_count($s, "a");
来源：http://hz.vqdsnc.cn/gtsrgzlxge.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtdggcqazl.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtubepidgf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ivvv.top/gtrdjaygbj.html

Go:   strings.Count(s, "a")
来源：http://hz.sufxvd.cn/gtlzjultft.html

Ruby: s.count("a")
来源：http://hz.smart0.xyz/gtmpltdbkk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.smart0.xyz/gtfzmmvmoa.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtnmpvcmjr.html

Py:   for ch in s: print(ch)
来源：http://hz.yvedp.cn/gttbitqpdv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guowangkeji.top/gtnscncwpq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtoyukqsur.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtpimlhgyw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yonumen.top/gtehxwkiyq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yueranfly.top/gtnirvstsw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hammf.cn/gtrjaavfuf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhongyouzk.top/gtgvodiwoh.html

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtshgrbrab.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xinyue.icu/gtkanhbmqx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hongshengwenyu.top/gtnumraiub.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtxyqbssoj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gtckrygmic.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tianlin.xyz/gtmkmsoqfp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangtech.top/gtxgtslhgt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shangyingyoupin.top/gtyeakzing.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtvchxbrkm.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gtzuplwtvj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gteknljkcw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtpwbykvbf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtarstzisc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.andypj.xyz/gtmfdqadzn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtrcisxcql.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.0kj1m.cn/gthaqtukbs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtjjrqneqr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtshtmknai.html

[E16] 数字千分位
来源：http://hz.feifeiyinyue.top/gtqoanptcb.html

Py:   f"{1234567:,}"
来源：http://hz.jiagoushi.top/gtgntawcgm.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gtsuxtnulf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gthnwzbriy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtakkjpljl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cheryme.top/gtuxrkjfll.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sxryk.cn/gtxiwdddld.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtmbgvckuv.html

C#:   1234567.ToString("N0")
来源：http://hz.pycfn.com/gtqujcwlmn.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtgrlmdqrl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.iojbl.cn/gtsvgqkgyg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gtcbsjnbys.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtagdixzhs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtzszxwjzp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtanvohfag.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jlsjyb.cn/gtryfarezz.html

Ruby: s.capitalize
来源：http://hz.cashguo.top/gtlpimiowo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gtsiwgroxd.html

[E18] 模板占位符替换
来源：http://hz.zhaomingkeji.xyz/gtvqismnti.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtzudpbzrj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtyastnrch.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtpzglfnye.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtcmwlqqqd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gthpwoesfw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.meibo888.top/gtfuluohne.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ywan-chungtsiang.top/gtlerloeam.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tanke756.top/gtgqwzmlgm.html

[E19] 多行文本按行拆分
来源：http://hz.haohaochexian.top/gtcrfphmcc.html

Py:   s.splitlines()
来源：http://hz.yuanzhike.top/gtfphphskp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fzhhl.top/gtsocthuwk.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtcmaawrqj.html

TS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtzwpvafar.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangtech.top/gtvejgsvop.html

Go:   strings.Split(s, "\n")
来源：http://hz.gaohongyu789.top/gtgtioqurq.html

Ruby: s.lines
来源：http://hz.ppjwa.cn/gtirznnljg.html

C#:   s.Split('\n')
来源：http://hz.vqdsnc.cn/gttdtvqnau.html

[E20] 判断字符串是否为空
来源：http://hz.jinyuanbaomall.cn/gthqmcflox.html

Py:   if not s:
来源：http://hz.nwbrower.top/gtqjaqujur.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zdqjudy.top/gtizpexnmp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtfcbbtpcv.html

TS:   if (s === "") {}
来源：http://hz.ivvv.top/gtqjiuqkpe.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtdpaaovul.html

Go:   if s == "" {}
来源：http://hz.andypj.xyz/gtkcvsforl.html

Ruby: if s.empty?
来源：http://hz.yonumen.top/gtkkqcmfel.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtdthfoqvm.html

[E21] 超长截断加省略号
来源：http://hz.yongpay.top/gthhpjhhfi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinghuilouyu.cn/gtjoysdyas.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gtiusgwgdy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtaivajobn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtkttvflrr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtcxddvums.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jyoumei.cn/gtvzpirqol.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtcghljzbq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtimgswkln.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gtsagrgsad.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nwbrower.top/gtgnwzpeel.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtbuengvru.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtefmezmkd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gteixlwptl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtsztqnmkh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtsqtscsuu.html

Ruby: s.bytesize;  s.length
来源：http://hz.meibo888.top/gthwlexayn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gttmereskm.html

================================================================================
来源：http://hz.9152youxi.cn/gtgzypndph.html

F. 文件与目录
来源：http://hz.bjfxy.top/gtwtskgulj.html

================================================================================
来源：http://hz.cucudq.cn/gtegvzpvco.html

[F01] 读取整个文件
来源：http://hz.yvedp.cn/gtlwdgvqom.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj202588.top/gtzmqzyvby.html

PHP:  file_get_contents("a.txt");
来源：http://hz.9152youxi.cn/gtmytugbil.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgufenzy.top/gtopuqrwjf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtzlvbhiqo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtkuclvznj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtaiodeqfs.html

Ruby: File.read("a.txt")
来源：http://hz.xinyue.icu/gtlxczmoab.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgufenzy.top/gtcafjuvfq.html

[F02] 逐行读取文件
来源：http://hz.cdnleiting.top/gtgjkecfwd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuxming.cn/gtkabctqlf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtfowfhkru.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gttuokejdu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtmtqadwig.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtkdvpbzvs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pycfn.com/gteeyfrlct.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258.top/gtipyxotgv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigufen.top/gtsqyohpyv.html

[F03] 写入文件（覆盖）
来源：http://hz.chenzaomai.com/gtbdjmcvjx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tian-w.cn/gtimlnbggh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtbhhaptrp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtwgxxeprt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtxxrfwmpg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gthrivhdul.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinghuilouyu.cn/gtxtbxonrw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.bjfxy.top/gtgdxctcrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtucjpkrfp.html

[F04] 追加写入文件
来源：http://hz.mhx1999.top/gtrssaossm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtrvfpqfsw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tian-w.cn/gtktalagek.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gttpqavvqs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtmxyoctjm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gtfbxrwpjt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daxiang520.top/gtxpmoapss.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtjkmdcdwf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtytmhiudo.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangshuangyany.cn/gtpirrsbnt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtqamdwzqh.html

PHP:  file_exists("a.txt");
来源：http://hz.vqdsnc.cn/gtetynqste.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtsnwaiyyu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtecepijzi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtyrzxltje.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtdwkkriyi.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gthgfbykfn.html

C#:   File.Exists("a.txt")
来源：http://hz.cucudq.cn/gtgvuyzoyt.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtclzuxihp.html

Py:   os.remove("a.txt")
来源：http://hz.zhongyouzk.top/gthnohxhlb.html

PHP:  unlink("a.txt");
来源：http://hz.hysaishi.cn/gtvssvdcwa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtrujucqvj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gthpynnwxj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtndxoiyrg.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtuhihbttm.html

Ruby: File.delete("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtsihdzpbo.html

C#:   File.Delete("a.txt");
来源：http://hz.c1oappe.top/gtmpgblhqp.html

[F07] 创建目录（含多级）
来源：http://hz.jiagoushi.top/gtgxzhozmk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtuwsqgfhu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtxytfzsot.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtiivlhtgg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtfythzzql.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtdcsmkzfa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.vqdsnc.cn/gtuwxeazcz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtsnxjrptj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtkfjvgsxo.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtrvncsett.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgfzy.top/gtpwygiddk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtxfjyrcpw.html

JS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtxvzbtaar.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtbwbzyaww.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtujvaaeem.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtltxrmpny.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtjdhhzxof.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtbpbkdmfn.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtjqtoohft.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ehwqpu.com/gtfsonfsgx.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtpufogawj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtouaokiwz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtxkgqsicx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtooawyegg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gtakinfzgh.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtgsgiwvpy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.haohaochexian.top/gtiepfdevs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zycfv.cn/gtzzrnbvzz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtjzsbrxxw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gzhubu.top/gtjpremzgf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtvhhnyvwo.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtofivswoj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dashuyun.cn/gtvvwcaykv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtlfcsgymw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtvneramqm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtnesqhcpa.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtlqlhsauw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtdohmsgsd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtwzcvvxwh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtrajrfcgt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtnjhoqlbb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daxiang520.top/gtffewhswg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ppjwa.cn/gtlyarebyh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtlgaltroy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258888.top/gtrhgmyjel.html

[F12] CSV 读写
来源：http://hz.zhongyouzk.top/gtywribhdy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtrdjhpvtv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhengqikj.top/gtwhwcxflm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtbrfevgyv.html

TS:   // 同上
来源：http://hz.cheryme.top/gtynypzrfx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aibaodan.cn/gtwairnmgg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgufenzy.top/gtbydkiezm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shzxlz.cn/gtziincluq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtjxfcuaep.html

================================================================================
来源：http://hz.guannengcc.top/gtsakbbhws.html

G. 面向对象
来源：http://hz.ywan-chungtsiang.top/gtzwdplznk.html

================================================================================
来源：http://hz.shzxlz.cn/gtmgjmscfk.html

[G01] 定义类
来源：http://hz.guannengcc.top/gtijlruqcf.html

Py:   class User: pass
来源：http://hz.cheryme.top/gttookvwbb.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtkcrmgiby.html

JS:   class User {}
来源：http://hz.cheryme.top/gtsadyzaji.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtwiavpopn.html

Java: class User {}
来源：http://hz.havefunace.top/gtehnfzejb.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtbcmnrtsq.html

Ruby: class User; end
来源：http://hz.xinyue.icu/gtkxqdycin.html

C#:   class User {}
来源：http://hz.gaohongyu789.top/gtjtulxiqg.html

[G02] 构造函数
来源：http://hz.shanyushiyangkeji.top/gttcscexkp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cucudq.cn/gtgeilpman.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fzhhl.top/gtinqljbut.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtwhtsdcjc.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtnloqchjw.html

Java: User(String name) { this.name = name; }
来源：http://hz.yvedp.cn/gtenrhrcnv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gthdszlkqk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtaxqttphx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gtbgvqfmlr.html

[G03] 实例属性
来源：http://hz.shanyushiyangkeji.top/gtdpxkcwwg.html

Py:   self.name = "x"
来源：http://hz.xinyue.icu/gtlxysbqrp.html

PHP:  public string $name = "x";
来源：http://hz.cqqwz.cn/gtxgoxaacu.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gtwhovfpym.html

TS:   name: string = "x";
来源：http://hz.cqqwz.cn/gtdvhfipkz.html

Java: private String name;
来源：http://hz.316326.xyz/gtxpxoykdd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gtxhgwjzkg.html

Ruby: @name = "x"
来源：http://hz.wangdashe.top/gtwbcjfgzr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtfjuocwru.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtpcxmlowb.html

Py:   def greet(self): return self.name
来源：http://hz.hongshengwenyu.top/gtauvczuoq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtgwusveim.html

JS:   greet() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtlbejcalj.html

TS:   greet(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtryjyhhyk.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtznzlttjb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hywenlv.cn/gthwxpzada.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtzplfwdtx.html

C#:   public string Greet() => Name;
来源：http://hz.dashuyun.cn/gtmuunjuyo.html

[G05] 继承
来源：http://hz.kuanghao11.cn/gtjpaokini.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtvimzqfqf.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtcbjbunua.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtnnjoiyaq.html

TS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtfexaxgxo.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gttnkjcvga.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuetiantiany.cn/gtqqpjkewv.html

Ruby: class Admin < User; end
来源：http://hz.cucudq.cn/gthkqctdwa.html

C#:   class Admin : User {}
来源：http://hz.gzhubu.top/gturmzrxrw.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gtamqpskmf.html

Py:   def greet(self): return "admin"
来源：http://hz.0kj1m.cn/gtsvgkseuq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtpmkrojav.html

JS:   greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtlapdtdjw.html


<!-- 参考信息 -->