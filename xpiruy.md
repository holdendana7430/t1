代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtwnklemmn.html

Java: String.format("%03d", 7)
来源：http://hz.chenzaomai.com/gtslcwhnqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nwbrower.top/gthjmljtzj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtifippxye.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtffgdvrtb.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtrooybrhi.html

Py:   s[::-1]
来源：http://hz.cheryme.top/gtwvfslhyd.html

PHP:  strrev($s);
来源：http://hz.daria6918.cn/gtvzdadazb.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gttqpgsowh.html

TS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtrvjybjlj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangshuangyany.cn/gtlhnsbwic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtqsoyisit.html

Ruby: s.reverse
来源：http://hz.jqgufenzy.top/gtsqlgrpcq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtkxhqtcnn.html

[E12] 统计某字符出现次数
来源：http://hz.pycfn.com/gtbgejusmh.html

Py:   s.count("a")
来源：http://hz.hysaishi.cn/gtrkfoerlq.html

PHP:  substr_count($s, "a");
来源：http://hz.jiagoushi.top/gthttjheew.html

JS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtrpnooumd.html

TS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtabmddirg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xziqi.cn/gtlibfebgu.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gthtkyqiys.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtfjxscaal.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jianghu66.top/gteedljboz.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gtwqoaixon.html

Py:   for ch in s: print(ch)
来源：http://hz.jinyuanbaomall.cn/gtxpnglboi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtnhrjdkaa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhijiandao.cn/gtsndanhby.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtdvpelyzi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.meibo888.top/gtispntspo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pycfn.com/gtuxwtqdkq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuanzhike.top/gtuqkacyzi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuanzx.com/gtstdbrlnv.html

[E14] URL 编码与 Base64
来源：http://hz.chenzaomai.com/gtetmpdchk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hongshengwenyu.top/gtksktbuax.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yangfankeji.com/gtbltbgpqd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gtvjttnuds.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dianchejie.cn/gtfhkyliga.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuanzx.com/gtenumnkro.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.svipenyu.cn/gtcbeaklui.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhaomingkeji.xyz/gtsocnnyan.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gtwldlakej.html

[E15] HTML 转义 / 反转义
来源：http://hz.tianlin.xyz/gtdyxvzvew.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hammf.cn/gtemeapauq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ywan-chungtsiang.top/gttbxbzmvx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.svipenyu.cn/gtmjngmcjl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gtuilmvxwk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tian-w.cn/gtkwdkygly.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gtcbdoccxf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cashguo.top/gtakvopxbq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtjyxgslml.html

[E16] 数字千分位
来源：http://hz.zhaomingkeji.xyz/gtribcdytq.html

Py:   f"{1234567:,}"
来源：http://hz.guowangkeji.top/gtbtfhoxbq.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gtzcwarlfg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtpwhkgpcz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtribizowf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtlnqkexpm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhengqikj.top/gtawltubea.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tian-w.cn/gtwwsymmhf.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxinkj.top/gtkrdwnxzn.html

[E17] 首字母大写
来源：http://hz.ydjk.org.cn/gtguqqhcvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fzhhl.top/gtbiwiuxcr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigufen.top/gtabzgtjul.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtojhoqjkg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhengqikj.top/gtvsbiljww.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtweyidjcz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hysaishi.cn/gtpxlxjvxd.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gtllhkkhoj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtkovlqnab.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtrfxgeowy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzhubu.top/gtvvhtkfom.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sufxvd.cn/gtrbnoisqk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gthgxpohfa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtwqyuqizo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtzafcjevv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gtsezozpww.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtoakfcorq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.mhx1999.top/gtylyhpnjc.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258.top/gtuccsmufv.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangkeji.top/gtkzebkjln.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhongyouzk.top/gthbbtsabe.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtkooxenpb.html

TS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtnalqptim.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gtvgzcdmap.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtzaabjbde.html

Ruby: s.lines
来源：http://hz.sweek.top/gtdajljphj.html

C#:   s.Split('\n')
来源：http://hz.zhijiandao.cn/gtgjwpsmnl.html

[E20] 判断字符串是否为空
来源：http://hz.jlsjyb.cn/gtpkpmzwje.html

Py:   if not s:
来源：http://hz.0kj1m.cn/gtoiggzrjr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtrodnawqd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtkfcveorb.html

TS:   if (s === "") {}
来源：http://hz.guowangkeji.top/gtitoflppa.html

Java: if (s.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtvuvqjknv.html

Go:   if s == "" {}
来源：http://hz.zhixingplan.top/gtmodehets.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtdwytdcwr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtovwwmkbc.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangkeji.top/gttrdlismr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtpkubshnx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgfzy.top/gtbclcmyez.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gttnlozzeu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtylkcrzwt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtjlnmywzb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gteauzofsf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zycfv.cn/gtycmoeruy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtwwykujfz.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gtrqttrufe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.haohaochexian.top/gtowjyosyz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtruraojyn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtcednlxri.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtecxewheu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gtyswlkfeg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xziqi.cn/gthbctclzv.html

Ruby: s.bytesize;  s.length
来源：http://hz.0kj1m.cn/gtgehoozhr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangdashe.top/gtzxkwomsb.html

================================================================================
来源：http://hz.wangshuangyany.cn/gttgximoyo.html

F. 文件与目录
来源：http://hz.daxiang520.top/gtvbnnunwr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpalpnwdc.html

[F01] 读取整个文件
来源：http://hz.yuxming.cn/gturqanuyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daria6918.cn/gtfdcqkaii.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtyndsrgrm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtryxhxrjk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtbkadhcbq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtnkvdekai.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigfzy.top/gtwlcxwblo.html

Ruby: File.read("a.txt")
来源：http://hz.nwbrower.top/gtgwaltfly.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinghuilouyu.cn/gtoziygshm.html

[F02] 逐行读取文件
来源：http://hz.pengpengdd.cyou/gtqeslqrpl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj202588.top/gthhvctrth.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hywenlv.cn/gtnervjhip.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtiusntdum.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtrdsvkfxw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtgojrgfus.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dashuyun.cn/gtxeyaqbtc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gttpkxshmq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gtljdhsgfu.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigufen.top/gtyhrvnjeb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cqqwz.cn/gtylvypjhv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gthbjohmdb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtqmdjwexm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtjswwyzmz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gttpwulcyo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtgsnsddid.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gaohongyu789.top/gtnwglagrf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuanzx.com/gtewdolxnq.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtkjatmjfl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yongpay.top/gtljhxuhvy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cdnleiting.top/gtlwwjsurg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtjpeldryh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtevaahlbf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gotoacloud.top/gtyuqnkcgy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.0kj1m.cn/gtxssrolsy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtzflsukeb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.mhx1999.top/gtbttzkrog.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gtfnnqexgi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtvcuwrhvq.html

PHP:  file_exists("a.txt");
来源：http://hz.fzhhl.top/gtglugqqyz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtgjnkgqrl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtytawjatl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtnwdomwdr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtwkfcfvmm.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinghuilouyu.cn/gtbvyvgdkb.html

C#:   File.Exists("a.txt")
来源：http://hz.hywenlv.cn/gtglgqtrqh.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtlfpqctrn.html

Py:   os.remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtgjfjqanp.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gtrgvchcfo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gthazeranf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtvajimcyc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtjdzwlpfn.html

Go:   os.Remove("a.txt")
来源：http://hz.gogol.net.cn/gtcuuntcdc.html

Ruby: File.delete("a.txt")
来源：http://hz.yuxming.cn/gtaltrajjt.html

C#:   File.Delete("a.txt");
来源：http://hz.9152youxi.cn/gtrhybdcvr.html

[F07] 创建目录（含多级）
来源：http://hz.havefunace.top/gtsetmhopm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtbfmsepod.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.0kj1m.cn/gtrklhtehf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtwnajaiep.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtawduopvn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtozgqwggq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhixingplan.top/gttfywdylg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.haohaochexian.top/gtcistwztw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuanzhike.top/gttgurkblh.html

[F08] 遍历目录
来源：http://hz.xuetiantiany.cn/gtejvwjuhc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.quarkkingdee.top/gtwigieikr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigufen.top/gttcijjmft.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtuamhwfox.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtkjfqowfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtxztziiqe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtczsjwewh.html

Ruby: Dir.children("dir")
来源：http://hz.jlsjyb.cn/gtphhkdjjd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.redwolf501.top/gtmbertpqz.html

[F09] 获取文件大小
来源：http://hz.smart0.xyz/gtlxwhwcgd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtdlqinvkm.html

PHP:  filesize("a.txt");
来源：http://hz.jianghu66.top/gtehkanygm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtweixnnvn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtembkioce.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtlrmuntdp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gtphlaghlb.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtxtoanvpc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtmeimmhck.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258.top/gtyxfhakwp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gttblmpbio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.bjfxy.top/gtnoazfkie.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtxjaauecv.html

TS:   path.extname("a.txt")
来源：http://hz.chenzaomai.com/gttxbqpxti.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guannengcc.top/gttxoelkpl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dianchejie.cn/gtkfclnhfa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtgekmiksi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gthgmbvdqd.html

[F11] 复制与移动文件
来源：http://hz.hysaishi.cn/gtounedtbj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtkfntxcbk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gttgvrwxtu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtopaysbvy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtnuahftjv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnqzz.top/gtyddpcmiv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fzhhl.top/gtvxwtqkps.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtjfeqfwih.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtnbeoedxs.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtxrnuirgb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtsdecdcxr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtdaubugol.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gtwnkytobi.html

TS:   // 同上
来源：http://hz.mhx1999.top/gtndpktdya.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtblkmiauh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtvglprcns.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhengqikj.top/gtowyqfqet.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guannengcc.top/gtcxandatm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtrorricrs.html

G. 面向对象
来源：http://hz.yvedp.cn/gtytmqynip.html

================================================================================
来源：http://hz.yj20258888.top/gtgnrezpgt.html

[G01] 定义类
来源：http://hz.zhoulong.xyz/gtxogofrkv.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtuuazeaxz.html

PHP:  class User {}
来源：http://hz.ivvv.top/gtbujfqket.html

JS:   class User {}
来源：http://hz.zhoulong.xyz/gtxurkoucn.html

TS:   class User { name: string = ""; }
来源：http://hz.sysykeji.top/gthfrrbujn.html

Java: class User {}
来源：http://hz.yj20258.top/gtxdmtbwwk.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtfwlphkzc.html

Ruby: class User; end
来源：http://hz.daria6918.cn/gtowzizlaa.html

C#:   class User {}
来源：http://hz.guowangkeji.top/gtrmwlwqoc.html

[G02] 构造函数
来源：http://hz.52xcode.cn/gtxgyossue.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gaohongyu789.top/gtcfzpqtiy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtreiwpzor.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gtfoxzapis.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gtpnfaccbd.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtrtvniksl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuxming.cn/gtdggvkwes.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtwebomtlq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtohurtckk.html

[G03] 实例属性
来源：http://hz.jqgufenzy.top/gtlaiqjoci.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtfkljojuh.html

PHP:  public string $name = "x";
来源：http://hz.9152youxi.cn/gtbjzcpele.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtqryyflxo.html

TS:   name: string = "x";
来源：http://hz.ybcxt.top/gthegddfuj.html

Java: private String name;
来源：http://hz.hnqzz.top/gtrmrntxyr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuxming.cn/gtntnxjspb.html

Ruby: @name = "x"
来源：http://hz.52xcode.cn/gtsuvmbqxv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtczoqicjg.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtzmcfqulp.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gteylefvnz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtxbbrbuvo.html

JS:   greet() { return this.name; }
来源：http://hz.cheryme.top/gtmtnmlwlr.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtupnpczew.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtcgfzcywt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtnphwevyt.html

Ruby: def greet; @name; end
来源：http://hz.smart0.xyz/gtywfcfsxt.html

C#:   public string Greet() => Name;
来源：http://hz.tanke756.top/gtwvfazvhc.html

[G05] 继承
来源：http://hz.yvedp.cn/gtvtyqtpqd.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtvqsoqaui.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtgwluzjuc.html

JS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtnyfiaxqf.html

TS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtivecccht.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtslbsbosl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtmlkjqmvr.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtgcrlzdwm.html

C#:   class Admin : User {}
来源：http://hz.zycfv.cn/gtrnrsjjce.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtgnydntmu.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtvmfdimel.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtjtknmmfp.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtjbmtdrrq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtfzpbanid.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtpgpijepc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtkspikglb.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gturlvrizs.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtujzyjhrj.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtfcbllwsh.html

Py:   super().greet()
来源：http://hz.andypj.xyz/gthbwwxtck.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtzvyygenu.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtnpweacpp.html

TS:   super.greet();
来源：http://hz.svipenyu.cn/gtfalqbrki.html

Java: super.greet();
来源：http://hz.tian-w.cn/gtcfadvvlw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtsfncirex.html

Ruby: super
来源：http://hz.yuanzhike.top/gtzjfkaesv.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtdyqcywvk.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtouqraafu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gtubgmtnqc.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtnogsqwmd.html

JS:   static f() {}
来源：http://hz.hfpthk.cn/gtferitape.html

TS:   static f(): void {}
来源：http://hz.yangfankeji.com/gtofkudqgk.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gtadlasdtq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yanxiufei.cn/gtzdcsqxex.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtvvnplgqo.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtfxkxthis.html

[G09] 接口 / 抽象类
来源：http://hz.kuanghao11.cn/gtodepfjvy.html


<!-- 参考信息 -->