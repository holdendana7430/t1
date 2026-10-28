代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hz.sufxvd.cn/gthszjfmmr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ywan-chungtsiang.top/gtdqajuaau.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigfzy.top/gtahexymgh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xziqi.cn/gtdjaluukm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.mhx1999.top/gtefiwcbdj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.feifeiyinyue.top/gtsynjtayb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.havefunace.top/gtspwzaern.html

JS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtumdqumwc.html

TS:   "7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtlufzyiyc.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtfddhvfws.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gaohongyu789.top/gtjntajxhj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pycfn.com/gtvakersvr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtjyyamdef.html

[E11] 反转字符串
来源：http://hz.pycfn.com/gtbbcdiayt.html

Py:   s[::-1]
来源：http://hz.pengpengdd.cyou/gtqnlnjbcv.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtxgzgiekp.html

JS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtpunlsetd.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtkssbtfxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj202588.top/gtjiqpxoan.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ehwqpu.com/gthbqtjdvx.html

Ruby: s.reverse
来源：http://hz.gogol.net.cn/gtsdzcwzbb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtfmwrnxca.html

[E12] 统计某字符出现次数
来源：http://hz.zycfv.cn/gtswxplabj.html

Py:   s.count("a")
来源：http://hz.vqdsnc.cn/gtbjrodzre.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtrohtzvwm.html

JS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gtlyhvsbzt.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtkzkzstlr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtkrimfmgx.html

Go:   strings.Count(s, "a")
来源：http://hz.zhaomingkeji.xyz/gtcfwbbuzb.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtnfmbizto.html

C#:   s.Count(c => c == 'a')
来源：http://hz.birdmap.top/gtcusprvti.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gtfwvoirvu.html

Py:   for ch in s: print(ch)
来源：http://hz.daria6918.cn/gtilcxbpdk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pengpengdd.cyou/gthvbbgggj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtawzypner.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtpygujzfw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guannengcc.top/gtrcrcvtsz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtgzjhwppt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shangyingyoupin.top/gtjyustyax.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gtohaswgei.html

[E14] URL 编码与 Base64
来源：http://hz.snrcjt.cn/gtljcawbre.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtpaaprubv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.haohaochexian.top/gtjrllvdle.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtvootijyl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gtlycygghw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gtmmgzaeuk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xziqi.cn/gthahebpik.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fengsongda.top/gtbaravjui.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangkeji.top/gtntavthcz.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtevphipoa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cheryme.top/gtxfupfydo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtiomdffvl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sweek.top/gtzmlfdtrb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtdqkypwws.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yongpay.top/gtwhctnjoq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtpaclkisy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtyyrmnpdi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtpvbpxlef.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gtxrewnpml.html

Py:   f"{1234567:,}"
来源：http://hz.yonumen.top/gtfvdywsed.html

PHP:  number_format(1234567);
来源：http://hz.zhijiandao.cn/gtaggovqwx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtmvzvychl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtotkuieus.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtyjjzgofu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dashuyun.cn/gtwpihdvbe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gthntutpjt.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gtnzzpxths.html

[E17] 首字母大写
来源：http://hz.dianchejie.cn/gtnfyqlguq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.havefunace.top/gtapdweapg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxinkj.top/gtmpglygzh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtykfcbgrd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtfydbclec.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.vqdsnc.cn/gtngwuhohr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gzhubu.top/gtoakyaehq.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtcbrjwjuu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhengqikj.top/gtbrnovxuz.html

[E18] 模板占位符替换
来源：http://hz.aibaodan.cn/gtflylqrxx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtgiyfmaju.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtrbssseam.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtjgudyjfw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtesmensda.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtlubqihey.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtgfvvkdse.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hammf.cn/gtwfbhnfqg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtcycrotub.html

[E19] 多行文本按行拆分
来源：http://hz.jianghu66.top/gtkiasoipx.html

Py:   s.splitlines()
来源：http://hz.shangyingyoupin.top/gtwsovldns.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pycfn.com/gtmmstttrt.html

JS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gthbncpsvp.html

TS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtxsgjcblx.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gtgypimvot.html

Go:   strings.Split(s, "\n")
来源：http://hz.sufxvd.cn/gtukmbuwcj.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtrzpszdim.html

C#:   s.Split('\n')
来源：http://hz.svipenyu.cn/gtvxrflbhf.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtabdfccxv.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtepbofeiz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gtzpovgbrl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtfzrgwxrw.html

TS:   if (s === "") {}
来源：http://hz.jqgufenzy.top/gthvxftuia.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtgwegfczu.html

Go:   if s == "" {}
来源：http://hz.smart0.xyz/gtfruqakum.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtbiauxekv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtmwguuofq.html

[E21] 超长截断加省略号
来源：http://hz.sxryk.cn/gtptxzkcbk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtjbjulbok.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gthitapncm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtzjlpqsap.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtfgvzbioc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtkygianml.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtizvbjpms.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gtjzudoghr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtcyfkxdpr.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtuzqlztjr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jianghu66.top/gtnwhtebut.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtffapqpam.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtjupydgdf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtiiexnalf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gtvmrunndx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhijiandao.cn/gtjlqtpyev.html

Ruby: s.bytesize;  s.length
来源：http://hz.fzhhl.top/gthnibscre.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhaomingkeji.xyz/gttjksilkj.html

================================================================================
来源：http://hz.jlsjyb.cn/gtiwyvthfb.html

F. 文件与目录
来源：http://hz.gzhubu.top/gtemzkypcm.html

================================================================================
来源：http://hz.tian-w.cn/gtmwwuwhwg.html

[F01] 读取整个文件
来源：http://hz.chenjidiqi.icu/gtoxjowwnm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtzyuglfpz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guowangkeji.top/gtyadxwkne.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenjidiqi.icu/gtnvfhmjoe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gaohongyu789.top/gtgowwrugp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtcnaohobo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigfzy.top/gtexkthafg.html

Ruby: File.read("a.txt")
来源：http://hz.sweek.top/gtmjriclry.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hongshengwenyu.top/gtkwvxkdye.html

[F02] 逐行读取文件
来源：http://hz.ppjwa.cn/gtootequhj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jianghu66.top/gtrveprbeg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtssqkqhwf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtwdgvhpvu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtzeqtssge.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtnqgzlrfk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.wangshuangyany.cn/gtwedqyqqn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.mhx1999.top/gtaevghrdb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ehwqpu.com/gtvnlgysiu.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gtjourkjxf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aizwys.cn/gthotofyvj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yvedp.cn/gtqymnrzbz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gttvijgxgl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtrziztxin.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtctoqstam.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dashuyun.cn/gtkcvdwqyz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xylfe.cn/gtakaydrud.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtwvpysube.html

[F04] 追加写入文件
来源：http://hz.wangdashe.top/gtwkymisuc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gttpbbamsi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fengsongda.top/gtgekkieku.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtysunvvff.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dianchejie.cn/gtcpwxokyl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuanzx.com/gtjjusinfg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aibaodan.cn/gtyxbabnen.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtwyjxcujm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.birdmap.top/gtearykmlg.html

[F05] 判断文件或目录是否存在
来源：http://hz.cdnleiting.top/gtmkhjejrq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ybcxt.top/gthylkzvwq.html

PHP:  file_exists("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtwcgynpce.html

JS:   fs.existsSync("a.txt")
来源：http://hz.svipenyu.cn/gtevvlenwf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtygyuamux.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtbcrpwwqu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.haohaochexian.top/gtpruczfaa.html

Ruby: File.exist?("a.txt")
来源：http://hz.fzhhl.top/gtfdonsilm.html

C#:   File.Exists("a.txt")
来源：http://hz.ybcxt.top/gtzxvzarcz.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtaclzvksa.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gtxovitytk.html

PHP:  unlink("a.txt");
来源：http://hz.nanxinkj.top/gtijdurmpu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigufen.top/gtpsugmezi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtjxsvydmn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtikdekpyi.html

Go:   os.Remove("a.txt")
来源：http://hz.xylfe.cn/gtelypwdos.html

Ruby: File.delete("a.txt")
来源：http://hz.9152youxi.cn/gtfswuqkcz.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtldatapwi.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtoywntwxr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtrolmprpp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zdqjudy.top/gttdloqinb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gthuthfmcz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtbhpiedbt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhijiandao.cn/gtnijoinso.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtzyxzkhco.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuxming.cn/gtxcwxmpgr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangtech.top/gtipadrhnx.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gteixhkpoe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtirhyfphu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yueranfly.top/gtwazlbwuh.html

JS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtedfqbddu.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gttdeugxkm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtnlfhkbja.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gttlmiscbk.html

Ruby: Dir.children("dir")
来源：http://hz.pengpengdd.cyou/gtvfjflgck.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtwmjbictr.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtofpwvblc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gtgpubsiea.html

PHP:  filesize("a.txt");
来源：http://hz.ydzc1.top/gtrhffmvuv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtvsvlsmzf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtsngduaid.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtkocsklly.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnqzz.top/gtpbeugpqm.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtupeopxno.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtauyvjbno.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtdkkuxqkd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtusasxzpy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cdnleiting.top/gtrgwqcptv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtqlcqgoik.html

TS:   path.extname("a.txt")
来源：http://hz.gogol.net.cn/gtvklnvtps.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhaomingkeji.xyz/gtlghsnved.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hammf.cn/gtsfswmsim.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtvilgigdu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtyitlaeex.html

[F11] 复制与移动文件
来源：http://hz.redwolf501.top/gtsmewblyo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtbegocasg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gtzjohgvjg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtpkvtkbji.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtrzanvvwr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtlcksvuud.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtpvlfeimo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtnhqvergx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.smart0.xyz/gtqywrlpkn.html

[F12] CSV 读写
来源：http://hz.havefunace.top/gttejwiizq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gtvdwqbedv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.kuanghao11.cn/gttaniqtaw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gtghiigwtk.html

TS:   // 同上
来源：http://hz.aibaodan.cn/gtwmqkatsf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtegirmmdo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hammf.cn/gtjxkjelvk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtekvanctq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jlsjyb.cn/gtjfzezcdg.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtrpuyjsvp.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtlixkskbz.html

================================================================================
来源：http://hz.yueranfly.top/gtyecapuvr.html

[G01] 定义类
来源：http://hz.52xcode.cn/gtmxyfgbqt.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtksroogjh.html

PHP:  class User {}
来源：http://hz.pengpengdd.cyou/gtedadyprt.html

JS:   class User {}
来源：http://hz.shuidangran.top/gtfodrjqct.html

TS:   class User { name: string = ""; }
来源：http://hz.meibo888.top/gtbhtsxmwq.html

Java: class User {}
来源：http://hz.hnxiangtu.top/gtbvfpsqok.html

Go:   type User struct { Name string }
来源：http://hz.jinyuanbaomall.cn/gtkjgjcbck.html

Ruby: class User; end
来源：http://hz.aibaodan.cn/gtkoxfctrd.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtrospeltz.html

[G02] 构造函数
来源：http://hz.yj20258.top/gtlwihspis.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gtzzcxxnpn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinghuilouyu.cn/gtnfrkokho.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangdashe.top/gtmrfoghar.html

TS:   constructor(public name: string) {}
来源：http://hz.chenjidiqi.icu/gtcgadygbl.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtwrhqtxft.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhongyouzk.top/gtcfaebswn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gttlmrrbyr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sufxvd.cn/gtbfsfqdby.html

[G03] 实例属性
来源：http://hz.yuxming.cn/gtzkvgxadx.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtxpkcavjx.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtfwiksemt.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtvmmvvikj.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtdrafhpsb.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtihovuuyz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hammf.cn/gtpftmzbwe.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gttdtbvpdz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gttoerirad.html

[G04] 定义方法
来源：http://hz.ehwqpu.com/gtdnhwycuo.html

Py:   def greet(self): return self.name
来源：http://hz.sweek.top/gtijfxlmsh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtjxwkcmaq.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtpyaxnumc.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj202588.top/gtqzjhhcnw.html

Java: String greet() { return name; }
来源：http://hz.pengpengdd.cyou/gtaicbobnk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtbkcpwgfr.html

Ruby: def greet; @name; end
来源：http://hz.yanxiufei.cn/gtswsjyzit.html

C#:   public string Greet() => Name;
来源：http://hz.shzxlz.cn/gtgygcdggc.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtdiidvfxc.html

Py:   class Admin(User): pass
来源：http://hz.nanxinkj.top/gtmgzjlzkw.html

PHP:  class Admin extends User {}
来源：http://hz.zhixingplan.top/gtabcrprlk.html

JS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtldahlqmw.html

TS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gttyohnktg.html

Java: class Admin extends User {}
来源：http://hz.sxryk.cn/gtepbfzvzv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.c1oappe.top/gtbbpksbdu.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtfquhjsir.html

C#:   class Admin : User {}
来源：http://hz.fengsongda.top/gtstieqnfy.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtrzpxtmxj.html

Py:   def greet(self): return "admin"
来源：http://hz.zhaomingkeji.xyz/gtrbmfzbtt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtelkydrlc.html

JS:   greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtripjudea.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtbmbxjizx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtclbfzgop.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtzjtfrzfj.html

Ruby: def greet; "admin"; end
来源：http://hz.smart0.xyz/gtwgxlgjgu.html

C#:   public override string Greet() => "admin";
来源：http://hz.pycfn.com/gtenjgnded.html

[G07] 调用父类方法
来源：http://hz.nanxinkj.top/gtshirrror.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtpoxhwmwd.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtvlwvvwkn.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtrysjejpq.html

TS:   super.greet();
来源：http://hz.tian-w.cn/gtfgrrmczw.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtzeemplua.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtsotaflmq.html

Ruby: super
来源：http://hz.zhijiandao.cn/gtaqbhitqy.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtlbfvikmm.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtpglhqwnt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtcwhkahqd.html


<!-- 参考信息 -->