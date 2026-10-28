代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dianchejie.cn/gtdchigqvi.html

[E11] 反转字符串
来源：http://hz.gogol.net.cn/gtftwehqwx.html

Py:   s[::-1]
来源：http://hz.c1oappe.top/gtjzkteueh.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gtgbwzlsqd.html

JS:   [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtbzxhdanm.html

TS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtaerbuvpm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aibaodan.cn/gtnfvwfypk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.haohaochexian.top/gtwglamwjb.html

Ruby: s.reverse
来源：http://hz.jqgufenzy.top/gtwdiqkapi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtfnihdoiu.html

[E12] 统计某字符出现次数
来源：http://hz.chenjidiqi.icu/gtyxhkuxyn.html

Py:   s.count("a")
来源：http://hz.daria6918.cn/gtqcyabkpz.html

PHP:  substr_count($s, "a");
来源：http://hz.dashuyun.cn/gtxyotyeed.html

JS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtsynyzuuh.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtowsbidfq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.9152youxi.cn/gtdytvssdh.html

Go:   strings.Count(s, "a")
来源：http://hz.hnqzz.top/gtjromclkp.html

Ruby: s.count("a")
来源：http://hz.hammf.cn/gtyvitilpb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gzhubu.top/gttexkfpah.html

[E13] 逐字符遍历
来源：http://hz.xinyue.icu/gtcqbtdqel.html

Py:   for ch in s: print(ch)
来源：http://hz.zhaomingkeji.xyz/gtnvceyovk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gtjvxukeix.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtksptgpcv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtydamuzso.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gthmzkbyso.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.mhx1999.top/gtousjawxc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj202588.top/gtnrwubjbl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.andypj.xyz/gtzmvfqxyx.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtbdfgpkcs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtmjxpnepu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gtwszynghq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yvedp.cn/gtthabbbfi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zdqjudy.top/gtdfvlflqt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.smart0.xyz/gtvmcyqbyc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sufxvd.cn/gtpeeotxxc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtjrwtnrpt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guannengcc.top/gtubqiavex.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gtdzcadhwm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shuidangran.top/gtfawllwig.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.andypj.xyz/gtvuyrqwml.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangkeji.top/gtaimxjula.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yonumen.top/gtcmjbhcfh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gttrmnncly.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydjk.org.cn/gtnwwtvdxw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gtgbibvpfx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aibaodan.cn/gtiddfqeqa.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtqrsvilsv.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtssrklcpk.html

PHP:  number_format(1234567);
来源：http://hz.jianghu66.top/gtfmxggbdg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtucrhnluj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtvdeacppx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtvwzugodi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ybcxt.top/gtiernlehq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtkzrbqlwu.html

C#:   1234567.ToString("N0")
来源：http://hz.yongpay.top/gtmiomapgm.html

[E17] 首字母大写
来源：http://hz.sysykeji.top/gtugwktzfd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhengqikj.top/gtfwkdqvxz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenlongwang.top/gtamxiydmo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtlsenogaq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtaamseupz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj202588.top/gtcszxzlao.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtnqjpkpip.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtyzbkymtt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhoulong.xyz/gtxzmttwiw.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtquzbgwsr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258.top/gtzpmmczhj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtajsrllmx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangshuangyany.cn/gtbdwqafyl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtbcrrfcaz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuanzx.com/gtryjxhuxz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yongpay.top/gtdwlfffsf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj202588.top/gtagrzihsh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tianlin.xyz/gtzzdivvjc.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtkwimwdmp.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gtuooseybm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigufen.top/gtrrlauipp.html

JS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtzgdvglrl.html

TS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gtcwrxbdxr.html

Java: s.lines().toList()
来源：http://hz.xuanzx.com/gtjpnxstsb.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxuanxn.top/gtfwuzxwxy.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gtxcfmqxmf.html

C#:   s.Split('\n')
来源：http://hz.c1oappe.top/gtjwhzlpnq.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtygeooequ.html

Py:   if not s:
来源：http://hz.ybcxt.top/gtwyhynnfi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtfzcafcdd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.andypj.xyz/gtwsxdpzil.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtxfawxrrr.html

Java: if (s.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtvtmgklpq.html

Go:   if s == "" {}
来源：http://hz.zhaomingkeji.xyz/gttkqroovg.html

Ruby: if s.empty?
来源：http://hz.gaohongyu789.top/gtmjrpwacz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.wangdashe.top/gtvrlxyust.html

[E21] 超长截断加省略号
来源：http://hz.xziqi.cn/gtlelcdxjw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtbfzpmrkz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gttxyjmwaq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtyxknkpys.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gttqnsyhzx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtkubqngrx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtxmmztdao.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xinyue.icu/gtjudxjiou.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtepalzvkc.html

[E22] 字节长度与字符长度
来源：http://hz.nanxuanxn.top/gtuycqbawt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtzxiozxfx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtbtmkkscn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtwoceeixa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gttbzrwuxq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gtjdftnnmd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ehwqpu.com/gtwipvdpig.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhijiandao.cn/gtvsrutiyg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gtmzuwotho.html

================================================================================
来源：http://hz.wangdashe.top/gtglgwhcof.html

F. 文件与目录
来源：http://hz.yuanzhike.top/gtxguhkovh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtpmgzmevh.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gthcxwzcit.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnqzz.top/gtlyvfuzza.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gtjbqyznek.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gtgngwjmzw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangshuangyany.cn/gtfskdqykd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtmlzhizqs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shangyingyoupin.top/gttsrvtwlc.html

Ruby: File.read("a.txt")
来源：http://hz.zhoulong.xyz/gthzwyoroc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ybcxt.top/gtimjliond.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtxdokpzvg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtxnphcjuo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtmvoyvudb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtbkwzeojg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gthxvmdxey.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtktsikyzm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.9152youxi.cn/gtmbvjiqxa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fzhhl.top/gtyoiezqwa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigufen.top/gteettydxz.html

[F03] 写入文件（覆盖）
来源：http://hz.ehwqpu.com/gtmvcvfora.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yangfankeji.com/gtnhlvgwwq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtizqejdex.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtjnfsiosu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gtlbmirxlp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtwhfyljrq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shzxlz.cn/gtjivpuqsz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gttgwuwdji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtodwjvume.html

[F04] 追加写入文件
来源：http://hz.snrcjt.cn/gtflrbkiyb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hfpthk.cn/gtxmutmlhd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sweek.top/gtmkobysjv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtejtkwosi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtuqikmsah.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xinyue.icu/gtvxqwvffp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtxwagimsg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shzxlz.cn/gtqhwjwkfb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtpuxmwusd.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtspkaqikf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yangfankeji.com/gtuwnjsybs.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtnzwlklip.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gteeeebdhi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtzcyimzlx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtznhmohxg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.9152youxi.cn/gtbrwzjjyo.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtywidibey.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtupbfkgtm.html

[F06] 删除文件
来源：http://hz.gaohongyu789.top/gtngcqaccq.html

Py:   os.remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtghaoyurw.html

PHP:  unlink("a.txt");
来源：http://hz.yuxming.cn/gtcggtfbvk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gtzdogyaen.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmrpqfcry.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtqnairdth.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gtluafwwnj.html

Ruby: File.delete("a.txt")
来源：http://hz.jyoumei.cn/gtwxnmriey.html

C#:   File.Delete("a.txt");
来源：http://hz.quarkkingdee.top/gtmbxuluho.html

[F07] 创建目录（含多级）
来源：http://hz.andypj.xyz/gtokyatjzh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtsdnujzxe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuetiantiany.cn/gtogrqkqst.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtrituliwc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtnwikpwag.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtdpazhuqw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guowangkeji.top/gtnunoabnl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtthfitswl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtckicjume.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gttmanwlwe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.snrcjt.cn/gtmierjana.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtjlkqpqdj.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtnkssfirm.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtmfnhamry.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtwijqutmx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtfkzyfeoe.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtnlzsxgfv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gttmkydqpd.html

[F09] 获取文件大小
来源：http://hz.zhaomingkeji.xyz/gtrxnvbatd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ppjwa.cn/gtzyqvehid.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtkrmaajqq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtpybkuadv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtfaowexau.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtsnxnxlyx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.andypj.xyz/gtjroglydk.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtexnhpgqh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cdnleiting.top/gtkdmstfzj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtmxcdlozh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtexmwcpwy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtomyqtvgw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtxqkdofti.html

TS:   path.extname("a.txt")
来源：http://hz.hnxiangtu.top/gthwatbvep.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gtulqbrypa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtdvcrnxug.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtptarjays.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hammf.cn/gtkwogwuqe.html

[F11] 复制与移动文件
来源：http://hz.yj20258888.top/gtaeartegk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtqhvrdhnb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gttaawhxds.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtbgumdlvc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtcobtsdof.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.kuanghao11.cn/gtfaoiwzeo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yonumen.top/gtqxtkwryu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtmgejbzmu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtxgxbgvjq.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtuerbsokj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aizwys.cn/gtyanqiqpe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gtgkwcedwz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.andypj.xyz/gtvwvruaoy.html

TS:   // 同上
来源：http://hz.meibo888.top/gtgyqowncz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xinyue.icu/gtamcalbkq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gogol.net.cn/gtjslglevp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtwgzzwbhl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtygrgzvhv.html

================================================================================
来源：http://hz.xinyue.icu/gtlkhbnrsx.html

G. 面向对象
来源：http://hz.aizwys.cn/gthvhknrou.html

================================================================================
来源：http://hz.andypj.xyz/gtczenwkao.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtkibsofmz.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtlpxjiiiz.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtxhgexlnk.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtqforkusw.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtnhxoyecj.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtuvxbuhin.html

Go:   type User struct { Name string }
来源：http://hz.jinqigfzy.top/gtzobydpaf.html

Ruby: class User; end
来源：http://hz.xuanzx.com/gtodqpszqv.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtxnaslbfh.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtathwolvn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtkfafjjwo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jyoumei.cn/gtzvracbvk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtqkzxhmrd.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gttzhsquru.html

Java: User(String name) { this.name = name; }
来源：http://hz.shuidangran.top/gtngyodeam.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtuiioqkhp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtbuqtmuni.html

C#:   public User(string name) { Name = name; }
来源：http://hz.andypj.xyz/gtysgolvmc.html

[G03] 实例属性
来源：http://hz.yongpay.top/gtamgjyfhj.html

Py:   self.name = "x"
来源：http://hz.kuanghao11.cn/gtrfuopxix.html

PHP:  public string $name = "x";
来源：http://hz.pycfn.com/gtqddxizge.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtubgarxig.html

TS:   name: string = "x";
来源：http://hz.hammf.cn/gtxkxwfsia.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtsqrpcqmg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtywwinvic.html

Ruby: @name = "x"
来源：http://hz.dashuyun.cn/gtpttagqmh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtnzdrzlhl.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gttugjqfoj.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtoojumfxc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtzujzmfeh.html

JS:   greet() { return this.name; }
来源：http://hz.iojbl.cn/gtephkcsan.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtiwmcxinz.html

Java: String greet() { return name; }
来源：http://hz.wangdashe.top/gtebqeznad.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtlnalqsic.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtmqvwrvkd.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtthecmena.html

[G05] 继承
来源：http://hz.mhx1999.top/gtvkiysvzo.html

Py:   class Admin(User): pass
来源：http://hz.guowangkeji.top/gtmjxhzffc.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtxycvzexr.html

JS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtxzubjbvs.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtpvlrjshf.html

Java: class Admin extends User {}
来源：http://hz.zdqjudy.top/gtncqesari.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhaomingkeji.xyz/gtmlzhippp.html

Ruby: class Admin < User; end
来源：http://hz.hfpthk.cn/gtwanktoky.html

C#:   class Admin : User {}
来源：http://hz.sweek.top/gtqtjssgop.html

[G06] 重写方法
来源：http://hz.zhixingplan.top/gtmkpfunth.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtawooemib.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtbxrgincr.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtkwjceexm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtsvvhoqnh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.havefunace.top/gtuujqaskn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xinyue.icu/gtyfivfhcc.html

Ruby: def greet; "admin"; end
来源：http://hz.yuxming.cn/gtjnvfxbqn.html

C#:   public override string Greet() => "admin";
来源：http://hz.iojbl.cn/gtrwivagsg.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtvflrdsuf.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gtbzjqcexl.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtqhdwarqo.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtjswsdavw.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtfwppdboq.html

Java: super.greet();
来源：http://hz.yj202588.top/gthuwwluzs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtfcpotmhj.html

Ruby: super
来源：http://hz.fengsongda.top/gtyztwlbyq.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtgmpzpcdx.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gtvstmpmhg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtrhyhkodl.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtranogohz.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gtdzogdgyh.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gttvccjoti.html

Java: static void f() {}
来源：http://hz.sweek.top/gtvdunhgcb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.svipenyu.cn/gtubshdbcp.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gtagofuijo.html

C#:   public static void F() {}
来源：http://hz.xziqi.cn/gtvzqwcinr.html

[G09] 接口 / 抽象类
来源：http://hz.meibo888.top/gtpfaviwhr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtnvabpycq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtsgznrlea.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jyoumei.cn/gtwwowmlyq.html

TS:   interface Shape { area(): number; }
来源：http://hz.hysaishi.cn/gtezzyumuj.html


<!-- 参考信息 -->