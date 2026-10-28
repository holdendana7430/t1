代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.ehwqpu.com/gtmbkevaei.html

Ruby: items.join(",")
来源：http://hz.zhengqikj.top/gtsyshyzkg.html

C#:   string.Join(",", items)
来源：http://hz.gogol.net.cn/gtyxiwbjeu.html

[E09] 去除所有空白字符
来源：http://hz.sxryk.cn/gteupzpjiz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangtech.top/gteyyxrywi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhengqikj.top/gtdbyhszwu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtdnprzrcn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gthfmqnktt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtrjjmfpgw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtvfajprwd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtqaycsplo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sxryk.cn/gtymaefkox.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtzharvjeh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtchwvxbzc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dashuyun.cn/gtbcbxkvkw.html

JS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtefwwjhhh.html

TS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtemjdmueo.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtxjgbyqol.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gogol.net.cn/gtzfrfnrci.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtwgkvuuja.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cucudq.cn/gtzzthwzke.html

[E11] 反转字符串
来源：http://hz.dianchejie.cn/gtznzjpyzp.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gtcjkqhbkb.html

PHP:  strrev($s);
来源：http://hz.tian-w.cn/gtbivqghcm.html

JS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtuolvrkgl.html

TS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtjyktfxye.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtbyxxwbsb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sufxvd.cn/gtxcymmlmi.html

Ruby: s.reverse
来源：http://hz.0kj1m.cn/gtuaspddjq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtadogvams.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtngpbgxlg.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtznvqafcu.html

PHP:  substr_count($s, "a");
来源：http://hz.haohaochexian.top/gtkafdxgth.html

JS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gtzqxwssed.html

TS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtszxsqgxp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.0kj1m.cn/gtpzzxqjam.html

Go:   strings.Count(s, "a")
来源：http://hz.mhx1999.top/gtddrlbwvs.html

Ruby: s.count("a")
来源：http://hz.nanxuanxn.top/gtzsnaeudr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gtwaveqbwb.html

[E13] 逐字符遍历
来源：http://hz.gotoacloud.top/gtzpucwymk.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtzopwsvdb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhijiandao.cn/gtcdoobdec.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtzfptpzkc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtyzjxcpap.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtyvwzjkto.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhijiandao.cn/gtbfbqrdex.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xingfuxueyuan.xyz/gtmbqrvujq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhongyouzk.top/gtaccgkcce.html

[E14] URL 编码与 Base64
来源：http://hz.shzxlz.cn/gtzrmchcik.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtplxalfwa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jyoumei.cn/gtqqdnciit.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gtgrpqjybd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtnjtodxpf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhengqikj.top/gtowlluwmd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhiwuduotai.top/gtfwnclzhy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shangyingyoupin.top/gtdeptvmkf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtalnnugkw.html

[E15] HTML 转义 / 反转义
来源：http://hz.birdmap.top/gtpdvibfgq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sweek.top/gtzoqvrogu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydzc1.top/gtrmkxjqtk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtimwudnfj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yueranfly.top/gtuwrqijbv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhoulong.xyz/gtwxsyfqlt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtdpttikyg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtugcswneg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sufxvd.cn/gtglivfdtj.html

[E16] 数字千分位
来源：http://hz.jianghu66.top/gtxknzoztc.html

Py:   f"{1234567:,}"
来源：http://hz.fzhhl.top/gtscjlyjsa.html

PHP:  number_format(1234567);
来源：http://hz.redwolf501.top/gtybeopsvr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dianchejie.cn/gtkyymndwr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtmerdzrzj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtvfoxqwmb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xziqi.cn/gtjzmeinou.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.havefunace.top/gtrxqhilpj.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gtlbiuoazw.html

[E17] 首字母大写
来源：http://hz.tanke756.top/gtkmmwbkem.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.kuanghao11.cn/gtmsnxetvt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258888.top/gtrhhafkmx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.meibo888.top/gtedwjmnii.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtbobzqymc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gteyksegvv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tanke756.top/gtrzlolngy.html

Ruby: s.capitalize
来源：http://hz.tanke756.top/gtioxczqtk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gtjdkvuwfi.html

[E18] 模板占位符替换
来源：http://hz.ydjk.org.cn/gtkzqdzbmc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zdqjudy.top/gtpgfwqees.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtmuxmfiil.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtmdvfkzwp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtjnbqqhet.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ppjwa.cn/gtdcvtzpfa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuetiantiany.cn/gtayftqlic.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yonumen.top/gtleezivok.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenlongwang.top/gtzrebfsio.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtusnhfnts.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangtech.top/gtyegqgkzx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.kuanghao11.cn/gtxzhjuqyl.html

JS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtobwexhrk.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtjyszuyqo.html

Java: s.lines().toList()
来源：http://hz.ybcxt.top/gtkxxeklyw.html

Go:   strings.Split(s, "\n")
来源：http://hz.xylfe.cn/gtyfhxqnzg.html

Ruby: s.lines
来源：http://hz.zhaomingkeji.xyz/gtbauzxlrn.html

C#:   s.Split('\n')
来源：http://hz.jinqigufen.top/gtsvlldbyr.html

[E20] 判断字符串是否为空
来源：http://hz.jqgufenzy.top/gtoffpqvwo.html

Py:   if not s:
来源：http://hz.wangshuangyany.cn/gtklmiouaf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenzaomai.com/gtjkcwnfjg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nwbrower.top/gtnoygzwiz.html

TS:   if (s === "") {}
来源：http://hz.nwbrower.top/gtpejoqcry.html

Java: if (s.isEmpty()) {}
来源：http://hz.yongpay.top/gtisokkgrr.html

Go:   if s == "" {}
来源：http://hz.jqgufenzy.top/gtajwkayts.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gtujjykoaq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gtkkmjfayp.html

[E21] 超长截断加省略号
来源：http://hz.nwbrower.top/gtwcibfwpl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgfzy.top/gtvnljpmtn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shuidangran.top/gtjaczbavs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtpurijzls.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtvymlvxcb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtkztbfqqq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenjidiqi.icu/gtflrsufhs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtkcnxsyfx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sysykeji.top/gtctdpwhcx.html

[E22] 字节长度与字符长度
来源：http://hz.aizwys.cn/gtjmdqueog.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gtpnlejvsq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.0kj1m.cn/gtyiejumxc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtvgiwgouw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtgmultdwm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtcjzkhauc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.52xcode.cn/gtklweuhgx.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtpjeqwvau.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtudpuqdgd.html

================================================================================
来源：http://hz.sxryk.cn/gttkmyagnm.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtztwmqpmp.html

================================================================================
来源：http://hz.yj20258888.top/gtwzbikbzz.html

[F01] 读取整个文件
来源：http://hz.nwbrower.top/gtpreiwmxi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtnwiysght.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shzxlz.cn/gtfcrrjneh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtbeusvvyo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtiwtykkmd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtfkhcptyg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.52xcode.cn/gtozygvxlw.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigufen.top/gtwprazpcl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hongshengwenyu.top/gtvhxfemzr.html

[F02] 逐行读取文件
来源：http://hz.kuanghao11.cn/gtscvlnvvc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hywenlv.cn/gtdehjsnrd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258.top/gtbluqersu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gthrwdwwbz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtokcpaamd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtsibvawob.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guowangkeji.top/gtgfqofatx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.9152youxi.cn/gtkaodeabv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cheryme.top/gtkwnwakgg.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtbahhoxwk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xziqi.cn/gtulpetygm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gzhubu.top/gtzcwleqka.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtomitevpf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtihrpwmbe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.birdmap.top/gtnffhvngw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dashuyun.cn/gtqygkfoac.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gtkojufjtw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtagmrrdqi.html

[F04] 追加写入文件
来源：http://hz.hysaishi.cn/gtspxweecs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shuidangran.top/gtsklqooqp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigufen.top/gtzbxtvycf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.52xcode.cn/gtdkfxrdzy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtihzbzxui.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dianchejie.cn/gtetextacv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtpmudvgys.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cashguo.top/gttnsxjrnq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dashuyun.cn/gthysjgmjh.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenjidiqi.icu/gtlvvzegho.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtzhczmtch.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigfzy.top/gtkinceedf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtrnrystnk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtlohkzjak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtjzcjjtmp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtklynzxlt.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenzaomai.com/gtdyzivahh.html

C#:   File.Exists("a.txt")
来源：http://hz.chenzaomai.com/gtjmbsdiwy.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtypgrtkbz.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtkxnmpqav.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtqcgpfmnq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtycnxmdie.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtsbblssfn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gttlsdkyvx.html

Go:   os.Remove("a.txt")
来源：http://hz.smart0.xyz/gtwzsrkeeo.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtpozvvqvt.html

C#:   File.Delete("a.txt");
来源：http://hz.zhongyouzk.top/gtyeoffgtf.html

[F07] 创建目录（含多级）
来源：http://hz.cqqwz.cn/gtgjcupwom.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtyacelqew.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtaqkfqvrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gteiqyuabf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtrcqrmgob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhiwuduotai.top/gtzazyrfqc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.svipenyu.cn/gtahmnqomh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gtxgjgwosw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtzvwgiroj.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gtcwpttakd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtsnuobizy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gtpzbrjakq.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtkmawujpw.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtkuatyotm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtzvwmfblc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gtogrqclyf.html

Ruby: Dir.children("dir")
来源：http://hz.mhx1999.top/gtvetxthhb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.smart0.xyz/gtmtecwvqu.html

[F09] 获取文件大小
来源：http://hz.andypj.xyz/gtsjzunrtq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtthcafiic.html

PHP:  filesize("a.txt");
来源：http://hz.zhijiandao.cn/gtctpluwdc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gthryhlrul.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtwkwhqfhr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtqrzuitoa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangshuangyany.cn/gtborccifw.html

Ruby: File.size("a.txt")
来源：http://hz.meibo888.top/gtezfmozxx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtpdolxpzi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gtawspwwwa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtnmsqckqz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sysykeji.top/gtydlyisly.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtwxdqxvtr.html

TS:   path.extname("a.txt")
来源：http://hz.yj202588.top/gtztkuycoj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtphodtxkh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtlbbexklg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtgfqyhebo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtdmbedljx.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtfmiehcnm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtddiexwks.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yonumen.top/gtxgsqkdol.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtfbpvfnca.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtmsiwryah.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtayretrcm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnxiangtu.top/gtvwogqgww.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtzofnkjtm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenjidiqi.icu/gtzyqfahku.html

[F12] CSV 读写
来源：http://hz.sweek.top/gtinkkkzkh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtmlltlagm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtevjdlivp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jyoumei.cn/gtmsnikjkx.html

TS:   // 同上
来源：http://hz.52xcode.cn/gtlxzjqgyx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtdwoyqcxk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtyxqxnrmz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gtpafgkzge.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.bjfxy.top/gtnthamkay.html

================================================================================
来源：http://hz.hfpthk.cn/gtvciptgur.html

G. 面向对象
来源：http://hz.jianghu66.top/gtpqxvhltn.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkgmrfqpg.html

[G01] 定义类
来源：http://hz.wangshuangyany.cn/gtcdywsohp.html

Py:   class User: pass
来源：http://hz.iojbl.cn/gtvvneiekw.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtkplgrjfe.html

JS:   class User {}
来源：http://hz.cucudq.cn/gtxwrfrorq.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtkgacsoaj.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtdmhhrnun.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtwoerglzi.html

Ruby: class User; end
来源：http://hz.xuanzx.com/gtnkfjhcfa.html

C#:   class User {}
来源：http://hz.yj20258888.top/gteddaecje.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtvkgyafsi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jlsjyb.cn/gtmqdlkevh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtmhdjckza.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gtfblylyus.html

TS:   constructor(public name: string) {}
来源：http://hz.52xcode.cn/gtxjcrqmbf.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangdashe.top/gtajowuxvi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtvpqxqdyd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtejazgtdn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenjidiqi.icu/gtshgzunji.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gthorwwbzb.html

Py:   self.name = "x"
来源：http://hz.jiagoushi.top/gtejyczzme.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtifpcjtcz.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gthdmbbjjy.html

TS:   name: string = "x";
来源：http://hz.yanxiufei.cn/gtyvydigrm.html

Java: private String name;
来源：http://hz.nwbrower.top/gtggdhjpvq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtvzcfhorb.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtlfkxeafp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj202588.top/gtxwwcezgl.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtaergftjl.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gthtaysgut.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtcovhlnge.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtoebtlucc.html

TS:   greet(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtwvndcdfg.html

Java: String greet() { return name; }
来源：http://hz.sysykeji.top/gtcmekbkpb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtveynvyxe.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtqpelnemt.html

C#:   public string Greet() => Name;
来源：http://hz.guannengcc.top/gtalavolcs.html

[G05] 继承
来源：http://hz.cucudq.cn/gttehklxoj.html

Py:   class Admin(User): pass
来源：http://hz.cdnleiting.top/gtzulmvgon.html

PHP:  class Admin extends User {}
来源：http://hz.jiagoushi.top/gtcrbishgy.html

JS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtxozopkcj.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gteiwwsvrt.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtasofrihe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cheryme.top/gtglcdgner.html

Ruby: class Admin < User; end
来源：http://hz.pycfn.com/gtphswbpil.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtnylguhqi.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gtchymyvdz.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigfzy.top/gtunznitnn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtpturpboj.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtolspqsos.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtzrawhgpu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gtqnvjowqk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtafbcwvqp.html

Ruby: def greet; "admin"; end
来源：http://hz.daria6918.cn/gtsigarkzj.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtlaaqbitz.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtdwxmmuki.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gthvhyikqz.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gttqzkkokn.html


<!-- 参考信息 -->