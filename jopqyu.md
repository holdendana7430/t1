代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.jqgufenzy.top/gtlmciqygo.html

Java: String.format("%03d", 7)
来源：http://hz.bjfxy.top/gtrkxzjzbf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxinkj.top/gtjfwazzuj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gtijnckkgg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hammf.cn/gtcnbpgibz.html

[E11] 反转字符串
来源：http://hz.meibo888.top/gtcnluksjc.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtpdctjbbq.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtmnsxqnpg.html

JS:   [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtvipartqm.html

TS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtryabuczz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jyoumei.cn/gtqweqkhwp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gtmnxphkgc.html

Ruby: s.reverse
来源：http://hz.zhiwuduotai.top/gtectrwiia.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtmrncxmaa.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gtmncfihvw.html

Py:   s.count("a")
来源：http://hz.316326.xyz/gtdbbkglyt.html

PHP:  substr_count($s, "a");
来源：http://hz.dashuyun.cn/gttdwuulwm.html

JS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtktprkxsk.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtncarmnzy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtjgscpjxc.html

Go:   strings.Count(s, "a")
来源：http://hz.haohaochexian.top/gtvtwwawke.html

Ruby: s.count("a")
来源：http://hz.bjfxy.top/gtqjutamls.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuxming.cn/gtccosmpcm.html

[E13] 逐字符遍历
来源：http://hz.9152youxi.cn/gtegrmrixh.html

Py:   for ch in s: print(ch)
来源：http://hz.wangdashe.top/gtkbyvnxek.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xinyue.icu/gtwrdzuvan.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.c1oappe.top/gtdkqpnjcz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtowdqjqie.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jianghu66.top/gtvomdrqua.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gzhubu.top/gtkenzdmbh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258888.top/gtutursrba.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtaiejcsvf.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gtdevsjhoq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258888.top/gtcdzubqdn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cheryme.top/gtjrznjwwl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aibaodan.cn/gtrfwoqqzq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhaomingkeji.xyz/gtbmjassgy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.iojbl.cn/gtvvejomwy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sweek.top/gtdakbxkjn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.smart0.xyz/gttdgzsvfl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnqzz.top/gtitfqafxx.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258888.top/gtsrnekshe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtufjguwdu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangtech.top/gtkuqtgxin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.meibo888.top/gtaugigixo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenlongwang.top/gtymgvlbbr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gtalyzkxmo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hfpthk.cn/gtmzymuprf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtctaokpno.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtymdlzzsd.html

[E16] 数字千分位
来源：http://hz.vqdsnc.cn/gtlxogpsxm.html

Py:   f"{1234567:,}"
来源：http://hz.zdqjudy.top/gtaubmywvf.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtzgkrqpkm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtvwzrkbmp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtdorylprs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgfzy.top/gtzbiviixb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtuwzcdewa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxinkj.top/gtejefmjdd.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gteomekcbm.html

[E17] 首字母大写
来源：http://hz.aibaodan.cn/gtiiqiubui.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtorkamxpw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtnbzjnfqo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtikorpunp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtgpwhnisz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hywenlv.cn/gtakhuwzhn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.mhx1999.top/gtbjvxgweu.html

Ruby: s.capitalize
来源：http://hz.hammf.cn/gtzlhqurqr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.0kj1m.cn/gtbforphki.html

[E18] 模板占位符替换
来源：http://hz.zhongyouzk.top/gtfazbafvd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhaomingkeji.xyz/gtotahjppe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xylfe.cn/gtxdzwmmra.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gthzuvvhme.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtvjvxvnkk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yvedp.cn/gtoxuqdxfn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtijnrnaeh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhaomingkeji.xyz/gtobrelsym.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pengpengdd.cyou/gtyhkriibl.html

[E19] 多行文本按行拆分
来源：http://hz.shzxlz.cn/gtylzdkimp.html

Py:   s.splitlines()
来源：http://hz.vqdsnc.cn/gtvtaovmnw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gaohongyu789.top/gtqyipcneg.html

JS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtueqihrcp.html

TS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtujyujmyl.html

Java: s.lines().toList()
来源：http://hz.feifeiyinyue.top/gtrxlrtrss.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxuanxn.top/gtgtbqccxm.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtbrbwochw.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtflktwozv.html

[E20] 判断字符串是否为空
来源：http://hz.hysaishi.cn/gtfeeftbfr.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtvpzpvmkl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtjgbkvnpb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtautorugs.html

TS:   if (s === "") {}
来源：http://hz.xingfuxueyuan.xyz/gtfuxtwxpc.html

Java: if (s.isEmpty()) {}
来源：http://hz.sxryk.cn/gtytedlogi.html

Go:   if s == "" {}
来源：http://hz.mhx1999.top/gtwaluoxkd.html

Ruby: if s.empty?
来源：http://hz.gaohongyu789.top/gtyxdzuxoj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.smart0.xyz/gtngftirtf.html

[E21] 超长截断加省略号
来源：http://hz.xuanzx.com/gthwfpvxml.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinqigufen.top/gtvhymqbuo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtuywurpsq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtoxjyyqil.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtinsxedvp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtiynytjjc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shzxlz.cn/gtamxsmyqp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigufen.top/gtqqliaywq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.9152youxi.cn/gtkcdgrnwc.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtbzleknlp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtcpmidbtx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtaiwcqqmb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtydavrfhx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtjgjfrtcn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtcskfmhfa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtqkafonej.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtsecirmwf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtewwuqkyl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtopmlwejj.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtowpijuwn.html

================================================================================
来源：http://hz.fzhhl.top/gtqblpybfo.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangkeji.top/gtsilssfzj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gthwipodue.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fzhhl.top/gteyomduze.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tanke756.top/gtnjmkfgco.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jyoumei.cn/gtwasscqdi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.meibo888.top/gttljxxkfk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daria6918.cn/gtopqrmqkt.html

Ruby: File.read("a.txt")
来源：http://hz.hnqzz.top/gtammttdvg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinghuilouyu.cn/gtlhmeqhzz.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gtssrmetna.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnqzz.top/gtshoayhqg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cheryme.top/gthnpymprv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtudmkiref.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtyqyfrwzn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtweptqflq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtcryebhti.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenjidiqi.icu/gttnfzykmb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtnsfllgsh.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gtwgczhgbf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhongyouzk.top/gtwlxgzclu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtbnctuklw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtywjztwzd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtkhfkplwe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigfzy.top/gtkzswamyk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.havefunace.top/gtapibsjyl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtvkarlyph.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xinyue.icu/gtshcfwsqz.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gthoqcldnp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.redwolf501.top/gtpzvsaouf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yueranfly.top/gtyikyxiht.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtgpgvdifp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtiqicwasx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fzhhl.top/gtezoyiafm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtbdocacqp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aizwys.cn/gtlvqgsdhd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gttzeqsyla.html

[F05] 判断文件或目录是否存在
来源：http://hz.gzhubu.top/gtuvgyghfe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.redwolf501.top/gtzmxtdyyu.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtqdetvzxy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtzuxnuitb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtzseujdus.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtrkrlnfyu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtpsrnlour.html

Ruby: File.exist?("a.txt")
来源：http://hz.cashguo.top/gtemtezhgs.html

C#:   File.Exists("a.txt")
来源：http://hz.daria6918.cn/gtcyzmkpux.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtpintcgpu.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtneuqtouq.html

PHP:  unlink("a.txt");
来源：http://hz.zhongyouzk.top/gtnnrjdchr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gttetqrgbr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtakpaamsj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtqoqgjdps.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtomtvttmx.html

Ruby: File.delete("a.txt")
来源：http://hz.ydjk.org.cn/gtnyngmjtp.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtayhpynvb.html

[F07] 创建目录（含多级）
来源：http://hz.xuanzx.com/gtipsunpxo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtjmbthjfi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cqqwz.cn/gtelmlqvxh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258.top/gtetseskda.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtxsglvmum.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtuaixcica.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhengqikj.top/gtloqjrjgg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gtsewbfwse.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hammf.cn/gtwtpkcynd.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtdguumwhn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhengqikj.top/gtzdcwbhyk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtjegxqdmv.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtlnvnsocc.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtozmrbnbq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtqqhxoacm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shzxlz.cn/gtyofkpsmq.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtmjdkxapl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gtglawtklr.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtabaxsxpa.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgfzy.top/gtyaiyjgqa.html

PHP:  filesize("a.txt");
来源：http://hz.gotoacloud.top/gtsukswndh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtckbjopak.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtsgwtjxeu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtcvfntmyd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fengsongda.top/gtzypqxgya.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gtfllyqasd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yongpay.top/gtbyvptxca.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtrfwxhzhn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtqotroged.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhixingplan.top/gtuintctud.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtxxzjnnmi.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtjcfscepi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtuhbfmdqn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtbnlcjcei.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gthblrbmeq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtewlfnmal.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtdvlsbjlq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtfpleqlod.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xingfuxueyuan.xyz/gtlomxvvhe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtwgodtynq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtfzmtmckz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gtwnikgjky.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtsvyqqdjl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtapqempcr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.feifeiyinyue.top/gttshxnjgk.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gttpicgvxk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jyoumei.cn/gtozojxkxs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtyvpraerw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtxonamxqz.html

TS:   // 同上
来源：http://hz.jinghuilouyu.cn/gtzalgfhdh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtdtnqsboa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gttrzjznbi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxuanxn.top/gthgzsaqlj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtupnnbios.html

================================================================================
来源：http://hz.316326.xyz/gtwdhubjcl.html

G. 面向对象
来源：http://hz.meibo888.top/gtmsvsctrq.html

================================================================================
来源：http://hz.aibaodan.cn/gtportdrgg.html

[G01] 定义类
来源：http://hz.zhixingplan.top/gtvnhgkfmn.html

Py:   class User: pass
来源：http://hz.sysykeji.top/gtjobeeunt.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtrzovwqrq.html

JS:   class User {}
来源：http://hz.vqdsnc.cn/gteoiacqxu.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtxmhqaljh.html

Java: class User {}
来源：http://hz.hywenlv.cn/gtxwvsfhyi.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtjyqpgfjw.html

Ruby: class User; end
来源：http://hz.zhixingplan.top/gtqbsxilbt.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtxvchbdyc.html

[G02] 构造函数
来源：http://hz.tianlin.xyz/gtymyznmmx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ppjwa.cn/gtpneqajir.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.meibo888.top/gtszwjqnsf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.andypj.xyz/gtfgyelyyr.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtmemcdefh.html

Java: User(String name) { this.name = name; }
来源：http://hz.aizwys.cn/gtjlpsbvlr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtfbdypgnk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtyeftpenx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yueranfly.top/gtarbkpias.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtsqhkoefs.html

Py:   self.name = "x"
来源：http://hz.ivvv.top/gtbfxmjmvr.html

PHP:  public string $name = "x";
来源：http://hz.xuetiantiany.cn/gtcakdkkqw.html

JS:   this.name = "x";
来源：http://hz.0kj1m.cn/gtojauhdcr.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtrydsoewq.html

Java: private String name;
来源：http://hz.c1oappe.top/gtprlcdkie.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.c1oappe.top/gtwauhrijo.html

Ruby: @name = "x"
来源：http://hz.zhaomingkeji.xyz/gtrubqfpdc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtihbneebn.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gttsuoybmt.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gtbvyqtbwd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtqqzrkywy.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtjhhyudkl.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtazxhlcvt.html

Java: String greet() { return name; }
来源：http://hz.ivvv.top/gtfvahevpr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.52xcode.cn/gtxivfumhr.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtjcgbzydf.html

C#:   public string Greet() => Name;
来源：http://hz.ybcxt.top/gtsfisujxg.html

[G05] 继承
来源：http://hz.smart0.xyz/gtdnprqvag.html

Py:   class Admin(User): pass
来源：http://hz.redwolf501.top/gtbjowdrlq.html

PHP:  class Admin extends User {}
来源：http://hz.gogol.net.cn/gtqymnypfx.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtpcydibau.html

TS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtptkozmyz.html

Java: class Admin extends User {}
来源：http://hz.cheryme.top/gtumxhkjsi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtuioqwwbp.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gtzlsuxcgj.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gtylhyvscb.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtczpssnwv.html

Py:   def greet(self): return "admin"
来源：http://hz.shzxlz.cn/gtxiloltvz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtiqxjnosb.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtvcqhwymq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtjxszphnu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtymishytr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yangfankeji.com/gtzowrxpdd.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtapusaajk.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtudemgmjd.html

[G07] 调用父类方法
来源：http://hz.yangfankeji.com/gtkpybkltw.html

Py:   super().greet()
来源：http://hz.dianchejie.cn/gtwcvrynji.html

PHP:  parent::greet();
来源：http://hz.yonumen.top/gtcuggdicg.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtlhmnlkus.html

TS:   super.greet();
来源：http://hz.yonumen.top/gtunpjhlgc.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gtnfxlszsb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtqegobcig.html

Ruby: super
来源：http://hz.sweek.top/gtpecyflkl.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtntfkvgdd.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtzsgyovnw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtirdbdwox.html

PHP:  public static function f() {}
来源：http://hz.ehwqpu.com/gtddasznlw.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtopnsdpyn.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtyumgwivo.html

Java: static void f() {}
来源：http://hz.cdnleiting.top/gthgssmdfn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtgpfhcctl.html

Ruby: def self.f; end
来源：http://hz.andypj.xyz/gtwkifdzho.html

C#:   public static void F() {}
来源：http://hz.shangyingyoupin.top/gtepclduxl.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtttuvubmg.html


<!-- 参考信息 -->