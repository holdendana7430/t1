代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtpfkmunct.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtyblhrhfl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.birdmap.top/gthfuuhwsk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dianchejie.cn/gtnrrymvik.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hammf.cn/gtwyudgkih.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hfpthk.cn/gtfeqpcjoz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtztkwbiqc.html

JS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtvtwnxyno.html

TS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtyonokirs.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gtfhfmabpz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtiltsupnr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tanke756.top/gtmnzvkofd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gtmgaabpuq.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtrfeetxre.html

Py:   s[::-1]
来源：http://hz.ydjk.org.cn/gtfmqlfcdr.html

PHP:  strrev($s);
来源：http://hz.xziqi.cn/gteemebgdi.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtgcvvrnnw.html

TS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtphfsdpbq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cqqwz.cn/gtsgtpvvpk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtaqzkoxdr.html

Ruby: s.reverse
来源：http://hz.zhaomingkeji.xyz/gtiziykniu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtkyfegjjp.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtvpdeqqfh.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtxleyahsp.html

PHP:  substr_count($s, "a");
来源：http://hz.shangyingyoupin.top/gtznqyxgdv.html

JS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtauqvgzcy.html

TS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtoywrtmtj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtgsutphoo.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtfkehbpnp.html

Ruby: s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtnmbqcqjv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxinkj.top/gtuquqalsi.html

[E13] 逐字符遍历
来源：http://hz.jinqigfzy.top/gtqicutxhl.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtynjmviar.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.mhx1999.top/gtwfdywjei.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtqrbcdmub.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.snrcjt.cn/gtcsxeznhh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuanzhike.top/gtvoaznixn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.mhx1999.top/gthikgnobv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtqnfkzceo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtqbofcgid.html

[E14] URL 编码与 Base64
来源：http://hz.pengpengdd.cyou/gtucddoboc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangtech.top/gtukqohwsu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fengsongda.top/gtyppnrzky.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gthxdyqqun.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinghuilouyu.cn/gtmbsczayz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtpwrmhhdv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xziqi.cn/gtjdytzzaz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtuukxljfq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtnzguwvgn.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigfzy.top/gtxkozxdpd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nwbrower.top/gtmooojxfe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yangfankeji.com/gtmrzblqih.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhongyouzk.top/gtusunjlut.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cdnleiting.top/gttwdwhope.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtveypszya.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnxiangtu.top/gtztntatau.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gteintcbmz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zycfv.cn/gtnxtmkega.html

[E16] 数字千分位
来源：http://hz.yongpay.top/gtbwxrauaa.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258.top/gtxmhzvwwi.html

PHP:  number_format(1234567);
来源：http://hz.sysykeji.top/gttvfllyma.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtnttmboul.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtgdhafkby.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.redwolf501.top/gtsjwijcal.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gtfiouyodm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jlsjyb.cn/gtmfgehpfi.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtmvytccfn.html

[E17] 首字母大写
来源：http://hz.guannengcc.top/gtfemdrwnl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtdxrzetcp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhongyouzk.top/gtegfxkqby.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtphhehago.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtzuvbeude.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtfydwdpdf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sysykeji.top/gtfcwrrszg.html

Ruby: s.capitalize
来源：http://hz.aizwys.cn/gtptpvrwhe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daria6918.cn/gtkdkmsbko.html

[E18] 模板占位符替换
来源：http://hz.jlsjyb.cn/gtgcygcchg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tian-w.cn/gttinxejsk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj202588.top/gtrwcgshzw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtuiozjlji.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtkcoxcgod.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jlsjyb.cn/gtmmshoage.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtxzohoxqi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jlsjyb.cn/gtvabljlhf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.meibo888.top/gtpzswobfb.html

[E19] 多行文本按行拆分
来源：http://hz.jinqigfzy.top/gtnalbfwts.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtewgiawqd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jlsjyb.cn/gtczyxshel.html

JS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtmnxgkyck.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtgpafkmsm.html

Java: s.lines().toList()
来源：http://hz.vqdsnc.cn/gtlgfleotp.html

Go:   strings.Split(s, "\n")
来源：http://hz.tanke756.top/gtucptydlu.html

Ruby: s.lines
来源：http://hz.yj202588.top/gtkvugcvxx.html

C#:   s.Split('\n')
来源：http://hz.zhengqikj.top/gtfdpuaqou.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtlbqswmgy.html

Py:   if not s:
来源：http://hz.c1oappe.top/gteqplbdvm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtouxispbq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.9152youxi.cn/gtgcwxpvsw.html

TS:   if (s === "") {}
来源：http://hz.svipenyu.cn/gtryexwyme.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gtmcyppxer.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gtrpttxqhx.html

Ruby: if s.empty?
来源：http://hz.xinyue.icu/gtjxdhgrjy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtwhijgmfe.html

[E21] 超长截断加省略号
来源：http://hz.quarkkingdee.top/gtkkvcgpop.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangdashe.top/gtmisgorbg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.svipenyu.cn/gtmvwuldny.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtrkbrclnp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtoevhwmql.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtogmlaboc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtseekdnhm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtssssvbgu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cqqwz.cn/gtcccnewwo.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangkeji.top/gtyczblhmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtqwnmvdnu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gtoosgjhae.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gthhcxtuun.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtfykcvkls.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guowangkeji.top/gtzlsbydvl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gtlpmmgbkf.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtnefakywq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zdqjudy.top/gtcmmxbpka.html

================================================================================
来源：http://hz.wangdashe.top/gtumwfgkqo.html

F. 文件与目录
来源：http://hz.nanxuanxn.top/gtbtfqpfvr.html

================================================================================
来源：http://hz.bjfxy.top/gtbkflamch.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtgtqchusm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtfnrynczh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cqqwz.cn/gtrmycuszr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shuidangran.top/gtsuwhigwu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.svipenyu.cn/gtliiirtlu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtfumkuwjl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtyajvglph.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtlkjqfjhw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxuanxn.top/gtmvwhascd.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtgrdxosjn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtisdyefxh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.vqdsnc.cn/gtkxewjens.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.kuanghao11.cn/gtngueywni.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gthklqleth.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtogyntjrq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgfzy.top/gtcpcqwefi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gzhubu.top/gtqlwjymup.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuetiantiany.cn/gtmaophowz.html

[F03] 写入文件（覆盖）
来源：http://hz.ehwqpu.com/gtbnmtfuho.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.smart0.xyz/gtwzpxslyb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jianghu66.top/gtepforfpf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtfyzqgzxh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtlfjvdkde.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.iojbl.cn/gtahdoymtr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtyfqsrblu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pengpengdd.cyou/gtehxitxou.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtsxspqtiu.html

[F04] 追加写入文件
来源：http://hz.xuanzx.com/gtgghyukxw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jyoumei.cn/gtwfrzxrck.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhaomingkeji.xyz/gtlvhpwerc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtjfdsfxwu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtgcgthmhh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtuhehyfyn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtdjvbftfy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj202588.top/gtuztcbayb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gturuuwoxm.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gthujzagzn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hammf.cn/gtamhdldce.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtzlidtdlc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.andypj.xyz/gttjzclrac.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtavhsvted.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtvbawqhyt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtovrkjbuo.html

Ruby: File.exist?("a.txt")
来源：http://hz.fengsongda.top/gtjoekkecr.html

C#:   File.Exists("a.txt")
来源：http://hz.hywenlv.cn/gtcyvbyfzy.html

[F06] 删除文件
来源：http://hz.sufxvd.cn/gtstntthfb.html

Py:   os.remove("a.txt")
来源：http://hz.ehwqpu.com/gtgpvxaewl.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gtulsfecco.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtksqwhsnw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gttcxlnqpx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtxyvdqxkv.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtyamwfqie.html

Ruby: File.delete("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtqenvfmtn.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtpkjgamlo.html

[F07] 创建目录（含多级）
来源：http://hz.chenzaomai.com/gtmlixcgbv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtujlxddbg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtpjfotbmj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtewshwkag.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtlbhvtypv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sysykeji.top/gtwybrvswy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenjidiqi.icu/gttiahuugz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.9152youxi.cn/gttifeflym.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.mhx1999.top/gtmyxprhrs.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gturqolddn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yangfankeji.com/gtqfychouj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shanyushiyangkeji.top/gtttvtmjty.html

JS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtznthpoyt.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtuaibcgbx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtkektwphg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tanke756.top/gttlxmfdys.html

Ruby: Dir.children("dir")
来源：http://hz.sufxvd.cn/gttigibdaz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.iojbl.cn/gtgbyhhqsc.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtzomllkku.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gtfxroglpt.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigufen.top/gtonvmfxbb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtcuebhrir.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtutmrlaeu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtyleswocd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtbzgctmxx.html

Ruby: File.size("a.txt")
来源：http://hz.shzxlz.cn/gtwmosllnp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtsqcmmkcx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtcorqvmob.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtstetbnna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xziqi.cn/gtwwjgpsbc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtqsheqquo.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gtfggsgthd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gtdghsqhui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtdgkvuxtg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtgotuguun.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtwuwhsjqp.html

[F11] 复制与移动文件
来源：http://hz.meibo888.top/gtbnrcdopg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtoioizraj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnxiangtu.top/gtqwxbgyky.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtouuzvdhj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtpkiuubhz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtwztisklm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtymeklfhn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtmqtlssxj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ehwqpu.com/gtemqsucij.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gtdqkmvpul.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.9152youxi.cn/gtaqgjduax.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aizwys.cn/gtxmxckzge.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tianlin.xyz/gtkcakbmpe.html

TS:   // 同上
来源：http://hz.sufxvd.cn/gtsmkgyuyc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtjvysdolw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.mhx1999.top/gtmnthxjja.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gtdpmwbrmd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ehwqpu.com/gtvevhxqgx.html

================================================================================
来源：http://hz.gzhubu.top/gtbnnjwocp.html

G. 面向对象
来源：http://hz.hnxiangtu.top/gtrnwjhdiv.html

================================================================================
来源：http://hz.9152youxi.cn/gthsqbrukd.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtttniijqt.html

Py:   class User: pass
来源：http://hz.gaohongyu789.top/gtavappfny.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtsavefack.html

JS:   class User {}
来源：http://hz.jqgufenzy.top/gtzueotnbj.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gtozqigfiu.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtijmkhvhe.html

Go:   type User struct { Name string }
来源：http://hz.ehwqpu.com/gtewkgzlwg.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtcsznupse.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtyyylumis.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gtqwzqgiae.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gthyyzqpcn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtohlkjvkj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtfkwqimta.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtbnzdbjrw.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtvljzmrih.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtgubamkzf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtfrfvwwdq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gtiqfcydls.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtyrndlbfn.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtwjfnjdgz.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtszusphrm.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtlmlftwli.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gtwtzjwrxw.html

Java: private String name;
来源：http://hz.zhiwuduotai.top/gtxurgpxyd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hammf.cn/gtkimdwtnx.html

Ruby: @name = "x"
来源：http://hz.9152youxi.cn/gtngytamgc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtgzlxieog.html

[G04] 定义方法
来源：http://hz.yj202588.top/gtdlmhvwwq.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gtfyxjcekc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guannengcc.top/gthbjzktyr.html

JS:   greet() { return this.name; }
来源：http://hz.ydjk.org.cn/gtashwpicd.html

TS:   greet(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtjshtuxvy.html

Java: String greet() { return name; }
来源：http://hz.svipenyu.cn/gtovwdptct.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtzjpwtzeb.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtdpbsyoan.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtkipcidmh.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtohudofex.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtmobtcoeu.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gthgnhyqfd.html

JS:   class Admin extends User {}
来源：http://hz.jqgfzy.top/gteeexgsku.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtgfszrkeh.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtobdnmggm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.52xcode.cn/gtdmukwxbx.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtnqrukjit.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtevypapcs.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtxcjyyxqj.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gteqihpojf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtfmrwrkls.html

JS:   greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtxpkxxtfb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gturafyjwh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtnwsygirc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gtyapwmeuh.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtmtlhsgit.html

C#:   public override string Greet() => "admin";
来源：http://hz.meibo888.top/gtyrnvamzq.html

[G07] 调用父类方法
来源：http://hz.feifeiyinyue.top/gtidvygvcz.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtwwphcwbj.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gtykdhsbvj.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gtvjrehiad.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtcwalmutp.html

Java: super.greet();
来源：http://hz.yongpay.top/gtvfidvpgy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.vqdsnc.cn/gtkuthtqlv.html

Ruby: super
来源：http://hz.nanxinkj.top/gtcmuriifc.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtgymskbzc.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtulqibxra.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtdrrkuxhs.html


<!-- 参考信息 -->