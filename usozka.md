代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtlgyqdqrg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigufen.top/gtkfosvplp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ehwqpu.com/gtjpcnzccx.html

JS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gttygxynnp.html

TS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtghzbyqnw.html

Java: String.format("%03d", 7)
来源：http://hz.9152youxi.cn/gtniclvatp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cucudq.cn/gtmgrghirl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hysaishi.cn/gtthcmdlfn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xziqi.cn/gtgbpnrsty.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtwckqpcfv.html

Py:   s[::-1]
来源：http://hz.jinqigfzy.top/gtqutwrmfn.html

PHP:  strrev($s);
来源：http://hz.jyoumei.cn/gtoikjzykp.html

JS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtkozvforp.html

TS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtqetohhbg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtobvizoah.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.vqdsnc.cn/gtkgrwqbua.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gtzljxujvp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtbrpxrfgs.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtzkvqwhmx.html

Py:   s.count("a")
来源：http://hz.0kj1m.cn/gtkauweemt.html

PHP:  substr_count($s, "a");
来源：http://hz.c1oappe.top/gtgnkvdwzs.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtyctfkvaz.html

TS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtrnistxxx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gthsvpcabw.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtfwnmstwe.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtcouyblqi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.redwolf501.top/gtlkfsmzvt.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtvgsvfuuq.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtgdeemqeb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtgylotvlr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtfelrnymr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hongshengwenyu.top/gtvlvfaecb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtmundcgja.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shuidangran.top/gtdedufbxz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aizwys.cn/gtqslmispa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gogol.net.cn/gtuoxouckt.html

[E14] URL 编码与 Base64
来源：http://hz.ivvv.top/gtistcqpmv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtzjglgypp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tianlin.xyz/gtfpppgutf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258.top/gtofscabsf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hysaishi.cn/gtqswrmxfh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtmmqchapf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhaomingkeji.xyz/gtgtcpymrq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hysaishi.cn/gtzayceztk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cheryme.top/gtnadffgng.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhiwuduotai.top/gtngcqbkjr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sweek.top/gtjkxmocsc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenzaomai.com/gtuzjndyip.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gotoacloud.top/gtzgfynngk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gtneazqhqi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnxiangtu.top/gtivettibu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtwvoojigk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnxiangtu.top/gtiepvtmjv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gtvztklroa.html

[E16] 数字千分位
来源：http://hz.daria6918.cn/gtkgrigbsy.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtbnwxomtj.html

PHP:  number_format(1234567);
来源：http://hz.tian-w.cn/gtstmrpngb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtyjbmrolk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtrncojtdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangkeji.top/gtgobsdmyo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pycfn.com/gtbbrmgaix.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhixingplan.top/gtyjicbtww.html

C#:   1234567.ToString("N0")
来源：http://hz.haohaochexian.top/gtlwytrsrg.html

[E17] 首字母大写
来源：http://hz.iojbl.cn/gtyntprmxj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sysykeji.top/gteddzplhb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.haohaochexian.top/gtqptrhszz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtutumzurv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gttvjtvfnv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.mhx1999.top/gtyudoficz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ivvv.top/gtdcganodu.html

Ruby: s.capitalize
来源：http://hz.wangshuangyany.cn/gtguquxlhc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gtfxupdfht.html

[E18] 模板占位符替换
来源：http://hz.nanxuanxn.top/gthywglrlp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sxryk.cn/gtfatkoxwh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gtujkmkhkm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtckheudfo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gttvkrxobi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtwuffhmmt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtefymhtgt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gtwtcvelnj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gotoacloud.top/gtdkprgfda.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gtbxwqfgyj.html

Py:   s.splitlines()
来源：http://hz.316326.xyz/gtsegkkbhk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gtsjipmhal.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhaomingkeji.xyz/gtchjkfqua.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtmpukmnzu.html

Java: s.lines().toList()
来源：http://hz.nanxuanxn.top/gtdqxegfre.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhoulong.xyz/gtdwjkwzla.html

Ruby: s.lines
来源：http://hz.yuanzhike.top/gtgeqifhpe.html

C#:   s.Split('\n')
来源：http://hz.fzhhl.top/gtuemfxfdl.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtaxdjjgse.html

Py:   if not s:
来源：http://hz.9152youxi.cn/gtbanhotna.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tian-w.cn/gthefqqeye.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258888.top/gtzmpogydd.html

TS:   if (s === "") {}
来源：http://hz.aibaodan.cn/gtgsuhtjok.html

Java: if (s.isEmpty()) {}
来源：http://hz.iojbl.cn/gtuphxzavx.html

Go:   if s == "" {}
来源：http://hz.redwolf501.top/gtdbphsgfy.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtzuzifxng.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gzhubu.top/gtowhcmecg.html

[E21] 超长截断加省略号
来源：http://hz.xylfe.cn/gtobwoqmsj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangshuangyany.cn/gtbwigwsnk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cucudq.cn/gttgyfkypi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtctnnnpgc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtzupvibaz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtnofopwnv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigufen.top/gtsgqjytpu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtvnevkkgo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtccharjfq.html

[E22] 字节长度与字符长度
来源：http://hz.zhengqikj.top/gtxcuqgrfx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgfzy.top/gtbydukxnh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhixingplan.top/gtjsoitrsv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtolbewtfe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtxqhdvlmt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtmzuvhfir.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gtobmcmtho.html

Ruby: s.bytesize;  s.length
来源：http://hz.nwbrower.top/gtnwxsvuhq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.birdmap.top/gtarrntgce.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnexkczxn.html

F. 文件与目录
来源：http://hz.birdmap.top/gtgcytbpxx.html

================================================================================
来源：http://hz.ydjk.org.cn/gthavrvkgh.html

[F01] 读取整个文件
来源：http://hz.nanxuanxn.top/gtkokpdjlb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tian-w.cn/gtgfldbixi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gttdiomijb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtykefblkx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shangyingyoupin.top/gtuvezbwvu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtghumzqfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtxrrvxdbg.html

Ruby: File.read("a.txt")
来源：http://hz.hnqzz.top/gtxvdvwlhm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtjqnsfmyo.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtxwmuolmk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gttblvcoeb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtdpaqbdsd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtbumdyaqs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinyuanbaomall.cn/gtgspighup.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtaeioarhe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gtwnutrpdk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.quarkkingdee.top/gtcnsrafrq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtrhnhgiac.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgfzy.top/gtxhnscxys.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gtsceggfvn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yvedp.cn/gthfhewaoz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtzakqyytf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hammf.cn/gtogzwkmoi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.feifeiyinyue.top/gtxbajdhjp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtmdxbxxrx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dashuyun.cn/gtyakoltcl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtjcnwvueu.html

[F04] 追加写入文件
来源：http://hz.tanke756.top/gtsulqhyby.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtvpuaouwf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtcvtpcjvq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtxrthadcu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtfrqtgcjl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtxdxbuchm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.kuanghao11.cn/gtnpzvmate.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtcqbnwybs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuetiantiany.cn/gtkyhaxmeh.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuxming.cn/gtsulxozey.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigfzy.top/gtymwomnqk.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtqrjolgox.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtanicospz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtzryygsol.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtybzphupu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.snrcjt.cn/gtpizfgfsc.html

Ruby: File.exist?("a.txt")
来源：http://hz.andypj.xyz/gtzarvuunn.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtajuauenn.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtsscibgya.html

Py:   os.remove("a.txt")
来源：http://hz.jlsjyb.cn/gtnooentsn.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtguaotghm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtlimgfktn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtlmrwexkm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtjqbidnba.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtusvkhdas.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangtech.top/gtdrmvmjlv.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtylesorvx.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtfgvswgoc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daxiang520.top/gtzgcgdwhv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtzzwfuqqd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtkmpspzon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gttyfifcsu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.andypj.xyz/gtouusjhra.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtbxhbiyoy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258888.top/gtdugxmrcs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.9152youxi.cn/gtsbndpzsz.html

[F08] 遍历目录
来源：http://hz.shanyushiyangtech.top/gtlebziqjr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtjcypjojw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtbslfxcpr.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtdwzsylls.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtrkkwonni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtkyqkqvwk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhengqikj.top/gtgkqiknjh.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtkvmbljpx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtugkyxnrs.html

[F09] 获取文件大小
来源：http://hz.smart0.xyz/gtoovlkixp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhijiandao.cn/gtbkduirjw.html

PHP:  filesize("a.txt");
来源：http://hz.quarkkingdee.top/gtzwivwwxw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtzdojztqj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtmybzzols.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtljpwjoii.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pengpengdd.cyou/gtvxfweucs.html

Ruby: File.size("a.txt")
来源：http://hz.nanxinkj.top/gthhhuihbs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhixingplan.top/gtwfhpxxlz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gturhadkmn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gthmwlkkrm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.52xcode.cn/gtubyiiwli.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtldhtbcgk.html

TS:   path.extname("a.txt")
来源：http://hz.xylfe.cn/gtpafcyxpv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.havefunace.top/gtqonzxylp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtugnhmrpt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtqngplxsb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtyvxaaxyn.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtjmcrbgxq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtfcvhqwoe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yanxiufei.cn/gtelrmpves.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtfqqkryid.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtzkpnacfp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhaomingkeji.xyz/gtdcpxjaar.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtbmvyzfei.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gttvlneump.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtwfpstedh.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gtlzcrypaz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gtjdrxzsdd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhoulong.xyz/gtemtpbpfy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtmlbgtvzc.html

TS:   // 同上
来源：http://hz.tanke756.top/gtgqqbqkqo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gtktuaazbm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtlsirizdn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtqptyueue.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtylnuxqyr.html

================================================================================
来源：http://hz.hammf.cn/gtmdzvcdes.html

G. 面向对象
来源：http://hz.cqqwz.cn/gtkrtncdej.html

================================================================================
来源：http://hz.aizwys.cn/gtursxivvg.html

[G01] 定义类
来源：http://hz.jinyuanbaomall.cn/gtwvrflbmj.html

Py:   class User: pass
来源：http://hz.aizwys.cn/gtpaaxbbis.html

PHP:  class User {}
来源：http://hz.ydjk.org.cn/gtbhtusomd.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtjijuzkwh.html

TS:   class User { name: string = ""; }
来源：http://hz.dianchejie.cn/gtuscbpuqe.html

Java: class User {}
来源：http://hz.zycfv.cn/gtywdycqev.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gturrhcmah.html

Ruby: class User; end
来源：http://hz.ydjk.org.cn/gtuambrgbl.html

C#:   class User {}
来源：http://hz.yueranfly.top/gtdbgicixu.html

[G02] 构造函数
来源：http://hz.shzxlz.cn/gtstqeqgjv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hysaishi.cn/gtdogrpiyy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtkzfmbryz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zycfv.cn/gtdlljpshb.html

TS:   constructor(public name: string) {}
来源：http://hz.zhiwuduotai.top/gtzlbmpwrw.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnqzz.top/gtplgzfawq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xylfe.cn/gtbqvuhvog.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinyuanbaomall.cn/gtclzyjuyk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gthlpvffud.html

[G03] 实例属性
来源：http://hz.hywenlv.cn/gttroaodjd.html

Py:   self.name = "x"
来源：http://hz.shuidangran.top/gtrjzpggjo.html

PHP:  public string $name = "x";
来源：http://hz.jlsjyb.cn/gtsilibchh.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtslktbpvu.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtepnbqwmr.html

Java: private String name;
来源：http://hz.hysaishi.cn/gtjwdzcoww.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gterrkjisa.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtvhgybhii.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxinkj.top/gtbmbgqvhg.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtrwtjiaox.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtkfviykxh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.meibo888.top/gtyfdchshc.html

JS:   greet() { return this.name; }
来源：http://hz.ppjwa.cn/gtcsdqvxnx.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtgcfuofrr.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gthdjdoboa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtybbqfaos.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtmgcqrbkf.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtaqplvyga.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtqwzwkcah.html

Py:   class Admin(User): pass
来源：http://hz.ydjk.org.cn/gtegrefqqp.html

PHP:  class Admin extends User {}
来源：http://hz.iojbl.cn/gtqjnpstxa.html

JS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtsgekgrrl.html

TS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtetiudcaw.html

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtrmtvbgwg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtmkgyeihg.html

Ruby: class Admin < User; end
来源：http://hz.andypj.xyz/gtwlugejyb.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtiujxsxxk.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtrfmcueqj.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtnegaiwlm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtpldvlufu.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtempojabb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtfzwbfoex.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtmbtvrgsd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtdwrpgdps.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtgtokcvbd.html

C#:   public override string Greet() => "admin";
来源：http://hz.shangyingyoupin.top/gtlhfqfwiz.html

[G07] 调用父类方法
来源：http://hz.cucudq.cn/gtxaeamexy.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtptnyffmx.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtrafoyywu.html

JS:   super.greet();
来源：http://hz.sweek.top/gtvuogtlsd.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtxrpggrzj.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gtsoqbabww.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtswxwpamh.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtcffmljlw.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtfajglgmh.html

[G08] 静态方法与属性
来源：http://hz.jlsjyb.cn/gtagmmpdzj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtnamcklmo.html

PHP:  public static function f() {}
来源：http://hz.yj20258888.top/gtchzfhwmd.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtqrplqkaf.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtdihacuzr.html

Java: static void f() {}
来源：http://hz.jlsjyb.cn/gtnysnwqrh.html


<!-- 参考信息 -->