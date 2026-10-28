代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtbnrxonyy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtmdfmdinx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.snrcjt.cn/gtwidqgdli.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gthppnpklp.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtdnzjlqra.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtdvtexbqi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtyybrxszb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gtvqfpjuuq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenjidiqi.icu/gtisykipao.html

[E11] 反转字符串
来源：http://hz.cucudq.cn/gtxaawnaca.html

Py:   s[::-1]
来源：http://hz.ivvv.top/gtngmsattp.html

PHP:  strrev($s);
来源：http://hz.guannengcc.top/gtvjcledvi.html

JS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gttimosfwt.html

TS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtntztwtud.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.quarkkingdee.top/gtceizkqba.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zdqjudy.top/gthhmupgtt.html

Ruby: s.reverse
来源：http://hz.ydjk.org.cn/gtqkgdwpsi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtnxzwtvhg.html

[E12] 统计某字符出现次数
来源：http://hz.jinyuanbaomall.cn/gtxcxoiodd.html

Py:   s.count("a")
来源：http://hz.hnxiangtu.top/gtopxzpbcx.html

PHP:  substr_count($s, "a");
来源：http://hz.svipenyu.cn/gtpepsrqaf.html

JS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtdyqgljkg.html

TS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gthqtwpvoo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ppjwa.cn/gtuvquisss.html

Go:   strings.Count(s, "a")
来源：http://hz.redwolf501.top/gtadwmoogt.html

Ruby: s.count("a")
来源：http://hz.gzhubu.top/gtkppciyzq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtdtjspvwo.html

[E13] 逐字符遍历
来源：http://hz.nwbrower.top/gtvkfmpuio.html

Py:   for ch in s: print(ch)
来源：http://hz.pengpengdd.cyou/gtkohgmmnw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gtvootkbdy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yongpay.top/gtotctzlhk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtfgbxzykk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yongpay.top/gtivmjmait.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cashguo.top/gtqruvjjtx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtvehiodzq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gtfzvuzzhk.html

[E14] URL 编码与 Base64
来源：http://hz.hysaishi.cn/gtnwtuyulp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xingfuxueyuan.xyz/gtfwzhhhel.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtmgvifqhr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.smart0.xyz/gtjwsrvvtg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tianlin.xyz/gtcktsbmtb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gtnxccksje.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.smart0.xyz/gtduxoxcqq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fzhhl.top/gtassqcqrb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shuidangran.top/gtrgaelfcc.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtdrilqlnt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.birdmap.top/gtcwvpupxt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gtmcxtptnl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gtxatqgujq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtyvlimraw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gzhubu.top/gtoicdozep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinyuanbaomall.cn/gtqzlxeaub.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aibaodan.cn/gtebnbxfuh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yuanzhike.top/gtxmmqnfnn.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gtjjokucdl.html

Py:   f"{1234567:,}"
来源：http://hz.aibaodan.cn/gthuwperrz.html

PHP:  number_format(1234567);
来源：http://hz.yj20258888.top/gtxbzckwdo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtjuigoxau.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtfwyzcuxb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gaohongyu789.top/gtwlbklzvx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.316326.xyz/gtaezdzetu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gtsoekonmx.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangkeji.top/gtenlosnof.html

[E17] 首字母大写
来源：http://hz.xziqi.cn/gtjhpbsgmx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtbgskzdtp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daria6918.cn/gtkkpowbne.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtskrdyrxv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gtsfjlsklv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ppjwa.cn/gtvrykyuat.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ybcxt.top/gtlmvzyspq.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtqlgjqkok.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shuidangran.top/gthlfnrhwd.html

[E18] 模板占位符替换
来源：http://hz.zhijiandao.cn/gttcqnngvg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzhubu.top/gttmtqidks.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtehxdlsab.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gttamivnsb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtaqlpsock.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.316326.xyz/gtlkpjbadl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gtkibghsrn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sxryk.cn/gtqnmhqbjl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ywan-chungtsiang.top/gtluwlukcj.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtmfkoqhjz.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gtnffzxbhf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuanzhike.top/gtumcecygg.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtrnzzjfnu.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtsvrloqkv.html

Java: s.lines().toList()
来源：http://hz.mhx1999.top/gtesomzqig.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtjfbplzme.html

Ruby: s.lines
来源：http://hz.iojbl.cn/gtlfinsevg.html

C#:   s.Split('\n')
来源：http://hz.yj20258888.top/gthrvkzgya.html

[E20] 判断字符串是否为空
来源：http://hz.cucudq.cn/gtizznazoh.html

Py:   if not s:
来源：http://hz.sysykeji.top/gtpgociymb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ppjwa.cn/gtfsgkkvyo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gaohongyu789.top/gtbbhkihgm.html

TS:   if (s === "") {}
来源：http://hz.tianlin.xyz/gtjbdcomxw.html

Java: if (s.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtbzmoxolo.html

Go:   if s == "" {}
来源：http://hz.shangyingyoupin.top/gtqkpwdtrm.html

Ruby: if s.empty?
来源：http://hz.yj20258888.top/gtjmmkpxlm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jiagoushi.top/gtjigvzsvl.html

[E21] 超长截断加省略号
来源：http://hz.ivvv.top/gtbzhocvtl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangkeji.top/gtfzyyrcyy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tianlin.xyz/gtkiiwgxag.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtrxqojkzj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtcehonzll.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtjcvvpsxv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.0kj1m.cn/gtvahjhbye.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.bjfxy.top/gtpkohcgos.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.quarkkingdee.top/gtrfnujtli.html

[E22] 字节长度与字符长度
来源：http://hz.yj202588.top/gtyfukgtjm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhixingplan.top/gtvspuxnss.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtymcwpaya.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtnhatrwjc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtcexftnwr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhoulong.xyz/gtcnxzhsdd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fzhhl.top/gtczkkqyth.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtykgbwayy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.mhx1999.top/gtlujjwynw.html

================================================================================
来源：http://hz.jqgfzy.top/gttlgrxydo.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtfirolwqv.html

================================================================================
来源：http://hz.havefunace.top/gtsihwoboe.html

[F01] 读取整个文件
来源：http://hz.daxiang520.top/gtkoajnher.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtwsclaxde.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jlsjyb.cn/gtxvkldxzj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghu66.top/gtdpeoanhs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.52xcode.cn/gtvwqkljiu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtbjfvutif.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuetiantiany.cn/gtwdgzpnjw.html

Ruby: File.read("a.txt")
来源：http://hz.52xcode.cn/gtsudzmbhq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangtech.top/gtzinbojrk.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtqeemstkr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangshuangyany.cn/gtqmbswtgy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cheryme.top/gticokzftd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gteogqinby.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtyszaglxs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtfwonttbv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yvedp.cn/gtnygsduig.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jiagoushi.top/gtyqrnjlbo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtmoxbfukp.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtlmddygcm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxinkj.top/gtchxauwkz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtmkplxiil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtpmgtbxzg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtvsgvqvdw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtwrqfkjzw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtockckbsv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xingfuxueyuan.xyz/gteyivggth.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtwsqzntyg.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtfqcaonvk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gthrxrkyop.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jyoumei.cn/gtmutdlktj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtyuvupyxf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtqvgkqymo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinghuilouyu.cn/gtdontfhhf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtkiraktst.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtahoekqvi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtwggtrdwy.html

[F05] 判断文件或目录是否存在
来源：http://hz.pycfn.com/gtspbzmwue.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtwviltdtl.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtjaiwsynq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtlpdfvblp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtuuvwfhit.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtsloknavn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sufxvd.cn/gtueaiimhf.html

Ruby: File.exist?("a.txt")
来源：http://hz.jiagoushi.top/gtcdxlibxr.html

C#:   File.Exists("a.txt")
来源：http://hz.hywenlv.cn/gtxgmnexzt.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gtvqixmdht.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtqrtuhpjr.html

PHP:  unlink("a.txt");
来源：http://hz.yuanzhike.top/gtedmkaxaq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtjpfkgorx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtnjhgstsg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtzlpenngt.html

Go:   os.Remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtvfgofbyb.html

Ruby: File.delete("a.txt")
来源：http://hz.dianchejie.cn/gtktespdpb.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gtpibyvgsj.html

[F07] 创建目录（含多级）
来源：http://hz.wangshuangyany.cn/gtqwuivfgg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtuhwulliu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gogol.net.cn/gtrnfuemhq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtprcqylse.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtifncpyoi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jlsjyb.cn/gtjxksbduj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shanyushiyangkeji.top/gtyxlqclkb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yvedp.cn/gtouernzrf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tanke756.top/gtzikcmvrw.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtxquulrnx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangtech.top/gthzyhpioz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fengsongda.top/gtuekcusbk.html

JS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtvigxcxfi.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtjabhnyee.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtxvcjqxum.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtnkmockzw.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtbewiabfn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtamfikhrs.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtpsdkgsyj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenlongwang.top/gtebkcrktf.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtiuqlnjhy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtybahthep.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gthgehzfwi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtjfnxnguw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fzhhl.top/gthndtywrp.html

Ruby: File.size("a.txt")
来源：http://hz.tian-w.cn/gtgxuykckz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtzybdhrtq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtyjpxwvdy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtqgfpqxrs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xylfe.cn/gtpcczubeh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtnzhslzyf.html

TS:   path.extname("a.txt")
来源：http://hz.yuxming.cn/gtlrazquaa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pycfn.com/gtfltdikpb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtdpodgwrv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtvoxighrw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtdmbalgyy.html

[F11] 复制与移动文件
来源：http://hz.cdnleiting.top/gtauwcdezx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtvffhcsws.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhoulong.xyz/gtqpvekruy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtltwljffa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtviejqrre.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtjwmncbhp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhaomingkeji.xyz/gtxgjkrgkd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtfgmtvsvm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.0kj1m.cn/gtrpyxpcas.html

[F12] CSV 读写
来源：http://hz.ppjwa.cn/gtjykeuphx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gtrnhohpsp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtysjoakfk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtwcfnknlb.html

TS:   // 同上
来源：http://hz.aizwys.cn/gtymkrlkix.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yuxming.cn/gtuzbsrxzp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yonumen.top/gtpkgggtzs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtbamdnnfp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fengsongda.top/gtppgkhgfk.html

================================================================================
来源：http://hz.ivvv.top/gtrpzsskvz.html

G. 面向对象
来源：http://hz.cashguo.top/gtcandctmm.html

================================================================================
来源：http://hz.yonumen.top/gtojpyqejk.html

[G01] 定义类
来源：http://hz.tanke756.top/gtlvlgffmx.html

Py:   class User: pass
来源：http://hz.zhoulong.xyz/gtnvnphemm.html

PHP:  class User {}
来源：http://hz.yongpay.top/gtybgmaxxb.html

JS:   class User {}
来源：http://hz.yj20258.top/gtoxvbyhla.html

TS:   class User { name: string = ""; }
来源：http://hz.zhengqikj.top/gtngohgypy.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtdmooerna.html

Go:   type User struct { Name string }
来源：http://hz.hfpthk.cn/gtowuyeamc.html

Ruby: class User; end
来源：http://hz.aibaodan.cn/gtijmglimf.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtpubeouwq.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtuitaainh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gteokckdpy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtgckowgvv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtvaufkmno.html

TS:   constructor(public name: string) {}
来源：http://hz.hfpthk.cn/gtckscekqz.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtyepchbld.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtwduuahkt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gteheuifqm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtqlzebnha.html

[G03] 实例属性
来源：http://hz.yj20258.top/gtqwsnsfmx.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtuuqnorfz.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gtcnuigmhb.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gteezoquzx.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtngpepcpf.html

Java: private String name;
来源：http://hz.cucudq.cn/gtazkgllbb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.mhx1999.top/gtepfiqduk.html

Ruby: @name = "x"
来源：http://hz.svipenyu.cn/gttahnrnqd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtqfcenxej.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtibxlqvzr.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtddbukvko.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtbylpyvvm.html

JS:   greet() { return this.name; }
来源：http://hz.cdnleiting.top/gteikdzefj.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangdashe.top/gtxrvmrelj.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtzxscutsi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.meibo888.top/gtvdfkmakx.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtvffuzjup.html

C#:   public string Greet() => Name;
来源：http://hz.zhaomingkeji.xyz/gtivxqyftj.html

[G05] 继承
来源：http://hz.wangdashe.top/gtjviwbadi.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtjlpudkmy.html

PHP:  class Admin extends User {}
来源：http://hz.andypj.xyz/gttsxtrywq.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtfdfrlcau.html

TS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtekrxaale.html

Java: class Admin extends User {}
来源：http://hz.cdnleiting.top/gtbxtpxvmm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yongpay.top/gtgbctqyuh.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtvfsnkglz.html

C#:   class Admin : User {}
来源：http://hz.andypj.xyz/gtbogxhkkk.html

[G06] 重写方法
来源：http://hz.vqdsnc.cn/gtdihldmlp.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtmwadcffb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtbdjflhoa.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtbxellops.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtkhyvjxlm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gttdoxsane.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtddopqzgx.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gtfgafadct.html

C#:   public override string Greet() => "admin";
来源：http://hz.aibaodan.cn/gtugbkevoh.html

[G07] 调用父类方法
来源：http://hz.yangfankeji.com/gtuxlobals.html

Py:   super().greet()
来源：http://hz.316326.xyz/gtdqjzbmtb.html

PHP:  parent::greet();
来源：http://hz.gogol.net.cn/gthpaltfkz.html

JS:   super.greet();
来源：http://hz.zdqjudy.top/gtxlpwpicq.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gtjrnkckqs.html

Java: super.greet();
来源：http://hz.yonumen.top/gtziauqzdv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtftbmjdzc.html

Ruby: super
来源：http://hz.fzhhl.top/gtiskjynmb.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtpjcbcecx.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtsznekrjq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gthnjxoihr.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gtwtkpgorr.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gtpdwcrljp.html

TS:   static f(): void {}
来源：http://hz.gogol.net.cn/gtzsbnalcm.html

Java: static void f() {}
来源：http://hz.shanyushiyangkeji.top/gtminwkjep.html


<!-- 参考信息 -->