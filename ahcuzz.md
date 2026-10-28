代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.feifeiyinyue.top/gtyiedjwxg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cdnleiting.top/gtwtrrszle.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ivvv.top/gtyovpuuwx.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtzdzpcmcn.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtfchjipka.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtyoamwhmf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pycfn.com/gtdrtlqkeu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258.top/gtjsqpzphj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.svipenyu.cn/gtqikhuklp.html

[E11] 反转字符串
来源：http://hz.tanke756.top/gtftwkybws.html

Py:   s[::-1]
来源：http://hz.tianlin.xyz/gtibieeabl.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtnxmvdnot.html

JS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtyhtklbrb.html

TS:   [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtqdcbfeyc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.quarkkingdee.top/gtwpicjfas.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtjyifdqqd.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtmyfdoxvo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtcthfidai.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtwxdjwatc.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtsnkfloks.html

PHP:  substr_count($s, "a");
来源：http://hz.andypj.xyz/gttagahobo.html

JS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtkekvklul.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtjelkwkup.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tian-w.cn/gtotlxhsqg.html

Go:   strings.Count(s, "a")
来源：http://hz.pengpengdd.cyou/gtcoysudfz.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtjydifdcu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258.top/gtttuqsijb.html

[E13] 逐字符遍历
来源：http://hz.pengpengdd.cyou/gtbhlclknz.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gttzztegbn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ybcxt.top/gtcofozihb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gttiyfdxgb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtrxullqxy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.havefunace.top/gtyboftcxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnqzz.top/gtfbuxgkks.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhijiandao.cn/gtgfjsvcqo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zdqjudy.top/gtamvkjxru.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gtribuzoap.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cheryme.top/gtheaoemzl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gtowxvsjxy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtsvtozwqj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnxiangtu.top/gtzobywbut.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhaomingkeji.xyz/gtvvpusdty.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hywenlv.cn/gtnarvarqu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yvedp.cn/gtorfwpgmq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yvedp.cn/gtlwhnqeld.html

[E15] HTML 转义 / 反转义
来源：http://hz.smart0.xyz/gtnubzebij.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtldeyrshe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yonumen.top/gtojahuaez.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guowangkeji.top/gttbmmoyip.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhoulong.xyz/gtxoogcrua.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangdashe.top/gtgiixzsbt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.haohaochexian.top/gtdfnjcnao.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtnktqrujr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.haohaochexian.top/gtdgxiqadr.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtvbesapzd.html

Py:   f"{1234567:,}"
来源：http://hz.cucudq.cn/gtxnaqojlt.html

PHP:  number_format(1234567);
来源：http://hz.hnqzz.top/gttuktnzon.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtcmjoddgk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtyltfcheu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuanzx.com/gtxdgjdkbu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cashguo.top/gttxpvjmqa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aizwys.cn/gtwhnqppic.html

C#:   1234567.ToString("N0")
来源：http://hz.hywenlv.cn/gtnpukosof.html

[E17] 首字母大写
来源：http://hz.guannengcc.top/gtfcpnxemy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xziqi.cn/gtkdmzrpyr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtjmxmyqab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtbqofpznb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtcbpccoyg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nwbrower.top/gtjkycvzyq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tianlin.xyz/gtpiqgnuff.html

Ruby: s.capitalize
来源：http://hz.shanyushiyangkeji.top/gtmsxsyhzl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fzhhl.top/gteywkyttg.html

[E18] 模板占位符替换
来源：http://hz.hnxiangtu.top/gtrztbgyog.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtpqfikswc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtiwlfbxet.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtvqqgksxo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtwsizsaiu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtewuhpelw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtjbqpvlgl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sufxvd.cn/gtpqlkcwod.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtznvujydk.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtzpoojbvl.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtyfnaiqky.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtshoitowc.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtismkwzsm.html

TS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtldqckuha.html

Java: s.lines().toList()
来源：http://hz.haohaochexian.top/gtmpnrlksy.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhixingplan.top/gtclnwxhtd.html

Ruby: s.lines
来源：http://hz.shanyushiyangkeji.top/gtgmpjbyla.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gttlrhynjs.html

[E20] 判断字符串是否为空
来源：http://hz.ybcxt.top/gtimkxknyy.html

Py:   if not s:
来源：http://hz.xuanzx.com/gtuyykdahu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydzc1.top/gtzowdxcrn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhijiandao.cn/gtmgqjhiqg.html

TS:   if (s === "") {}
来源：http://hz.zhixingplan.top/gttbqnaaqv.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtvcqmdtgk.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtejdwkzsb.html

Ruby: if s.empty?
来源：http://hz.cucudq.cn/gtwxmatbhv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtcxnfupwf.html

[E21] 超长截断加省略号
来源：http://hz.jqgufenzy.top/gtqpydzxog.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtkelnymdp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtoekckyeh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtemgbyqvn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtuutdfcsn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtmbctdghv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.haohaochexian.top/gtyxurvwgi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.smart0.xyz/gtynqhntdx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtnttttgdf.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangkeji.top/gtsgoqnjeb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.snrcjt.cn/gtkigkvxfw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtryaqmfvr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gthwcriwba.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtcymubwxy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtxwmyvnkj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtfplncouw.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenzaomai.com/gtlvlalsas.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtkhkgvcfq.html

================================================================================
来源：http://hz.jinqigufen.top/gtsrcktzqu.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtqlssyiji.html

================================================================================
来源：http://hz.cucudq.cn/gtqsdbqjhr.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtdavhqijq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtqfmjzzmb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guowangkeji.top/gtlzfgzrwm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gtaeksrvxr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gteuyqfdwu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtigzpaady.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gttzjdjspc.html

Ruby: File.read("a.txt")
来源：http://hz.sysykeji.top/gtstnkrlzd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hysaishi.cn/gtbxqrwxkv.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gtwdslcttb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gthrgovyye.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hammf.cn/gtdofdbplz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtlprlowzz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtalehzwwc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xziqi.cn/gtisnmsjxo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yueranfly.top/gtjbclvfnv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtaofsqwla.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tianlin.xyz/gtohmidgkb.html

[F03] 写入文件（覆盖）
来源：http://hz.zhijiandao.cn/gtbizjkidq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gtkbccvaks.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtpnbexdui.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtxcmihfap.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtgrxnsnzc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gttbmiqdhl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtmrkeevzf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258888.top/gtjpghigtx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtvehjufqi.html

[F04] 追加写入文件
来源：http://hz.pengpengdd.cyou/gtzmefkson.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtjvphsxzg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yvedp.cn/gtnqqydpig.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtnpgfcknr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtmvuorbmv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gttmqgedtc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ydzc1.top/gtfyglqzao.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sufxvd.cn/gtsxprzqam.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhoulong.xyz/gtqnjdbqgk.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gtzcrgunks.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuetiantiany.cn/gtargdfpzx.html

PHP:  file_exists("a.txt");
来源：http://hz.jyoumei.cn/gtyzpmufii.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtxvwpohzh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtugjnkwbr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtoemadtgf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jiagoushi.top/gteixpkceb.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenlongwang.top/gtsmxlkqdn.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtllacywzy.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gtcnzsfwio.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtuuwnmisf.html

PHP:  unlink("a.txt");
来源：http://hz.sxryk.cn/gtcrlcmyau.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtgjgdrqff.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtmnqehixb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtbwqlfghj.html

Go:   os.Remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtdzjapizj.html

Ruby: File.delete("a.txt")
来源：http://hz.chenlongwang.top/gtvvmixiwa.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangtech.top/gtybyzqcxj.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtkhbnsvmh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gthqnijfwa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guannengcc.top/gtodhqkuey.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gttlqylijl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtkvzfciou.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtkzngebez.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.mhx1999.top/gtvxncybrw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtdstztmet.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtmdpelzvv.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtvesyeeax.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tian-w.cn/gtaqvlipsy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ppjwa.cn/gtnnkpiqfo.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtjytjxfza.html

TS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtuvwmuubz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yonumen.top/gtwkpyijqu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gtyzqawucc.html

Ruby: Dir.children("dir")
来源：http://hz.jianghu66.top/gtmxhsfuey.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtrtspgpin.html

[F09] 获取文件大小
来源：http://hz.haohaochexian.top/gtrlyvhcrm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnxiangtu.top/gtovrwiiur.html

PHP:  filesize("a.txt");
来源：http://hz.zhijiandao.cn/gtyaertnch.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtqcfjoumi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtmnfwiemr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gteygbjlxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtcmbwyapn.html

Ruby: File.size("a.txt")
来源：http://hz.c1oappe.top/gtarqfovec.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sweek.top/gtiuocbhgf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zycfv.cn/gttsztsxcs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtevqgtbbp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gtivjuikyu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtutzbbyfg.html

TS:   path.extname("a.txt")
来源：http://hz.zhongyouzk.top/gtzpxxirlm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gttmjwtita.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtvupxdkmj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtdzqjsben.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtpyzvprxu.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtrbslbmgj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtxdircbmt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cheryme.top/gteoeetatv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gteilkbtrp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtiiuzekpk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dashuyun.cn/gtujzurmvd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhengqikj.top/gttbyviwbx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtogohelfs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yonumen.top/gtxqahngly.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtqzksxdpz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gtmtxmhrom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gtoyvmlnkk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sweek.top/gtsekojcuy.html

TS:   // 同上
来源：http://hz.redwolf501.top/gtkojwvxjn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gtnjsckrnv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gthucxbfim.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sweek.top/gtartvmphk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtrmzdmkpv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtllnqzjok.html

G. 面向对象
来源：http://hz.hfpthk.cn/gtfhqynvwb.html

================================================================================
来源：http://hz.jqgfzy.top/gtpcgxxmhz.html

[G01] 定义类
来源：http://hz.yj202588.top/gtfxicyayr.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtfvjzhqjh.html

PHP:  class User {}
来源：http://hz.smart0.xyz/gtmiltxigv.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtxahyjsze.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtzkwlfhrg.html

Java: class User {}
来源：http://hz.chenjidiqi.icu/gtobcljgby.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtkowqplnt.html

Ruby: class User; end
来源：http://hz.redwolf501.top/gtkoivjmax.html

C#:   class User {}
来源：http://hz.chenjidiqi.icu/gtcwotvnes.html

[G02] 构造函数
来源：http://hz.jyoumei.cn/gtmrbvdkkj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtueutflkj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangtech.top/gtqbtpeult.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gthumrrpjz.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gtiidsswro.html

Java: User(String name) { this.name = name; }
来源：http://hz.bjfxy.top/gtlsfgkclu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gthluwlxss.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtdepbyxkm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daxiang520.top/gtlbuabwik.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtzvnsvajs.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtipwaucbc.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtfcxmzbbc.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtbukoslqo.html

TS:   name: string = "x";
来源：http://hz.gzhubu.top/gthytuflzp.html

Java: private String name;
来源：http://hz.316326.xyz/gtlfeglyur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtliolifjd.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtphsziufj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtsaixprwa.html

[G04] 定义方法
来源：http://hz.ivvv.top/gtnlpliyxr.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtoeurqijn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtxvcergnp.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtexdqavkt.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gthunprhug.html

Java: String greet() { return name; }
来源：http://hz.nanxuanxn.top/gtalkrcwvt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtwljabxir.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtebtnqsbp.html

C#:   public string Greet() => Name;
来源：http://hz.quarkkingdee.top/gtrezekwng.html

[G05] 继承
来源：http://hz.svipenyu.cn/gtgumyrnpf.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gtjzktkpqk.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtzpywzykc.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtdcifxkoc.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtgxhhlawj.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtgfphuhtv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.mhx1999.top/gtrqarqzek.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtjvmggfds.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtdgkitbye.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtmnkcleyl.html

Py:   def greet(self): return "admin"
来源：http://hz.hfpthk.cn/gtekvgbpxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtjdnufswc.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtvgxcbcal.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gttdzlxuyk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtpzbgkllm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sufxvd.cn/gtespiasip.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtlcabihxy.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gttuiteqif.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtbkqjolrb.html

Py:   super().greet()
来源：http://hz.yj202588.top/gtzjmlhcie.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtwoabivfq.html

JS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtdpnkbsyq.html

TS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gtducnmemz.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtajkaiccf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtpganremr.html

Ruby: super
来源：http://hz.nwbrower.top/gtbrbthios.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtfqphobbm.html

[G08] 静态方法与属性
来源：http://hz.yongpay.top/gtnhvalrmk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtzyrqrvct.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtgxqmkoif.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtayhditrk.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtauxiampy.html

Java: static void f() {}
来源：http://hz.jlsjyb.cn/gtdnwonndh.html


<!-- 参考信息 -->