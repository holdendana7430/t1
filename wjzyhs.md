代发 wailian999

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtkfmjdvhv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtdnffhtwk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtzvptzchh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtgzejowum.html

TS:   s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtqeffgosz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtjzuzrgfs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jyoumei.cn/gtjysbtvhr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sufxvd.cn/gtduyzwbqv.html

C#:   s.Replace("a", "b")
来源：http://hz.cqqwz.cn/gtzclniqfm.html

[E07] 按分隔符拆分
来源：http://hz.shuidangran.top/gtawrvoosq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jyoumei.cn/gteptuydwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yangfankeji.com/gtvzssjfkr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtfsjegdyd.html

TS:   s.split(",")
来源：http://hz.nwbrower.top/gtdyplmlsg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.iojbl.cn/gtbypxuxfr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.dashuyun.cn/gtdwlartsl.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangtech.top/gtfsmgxofn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zdqjudy.top/gtjivoyuhq.html

[E08] 数组按分隔符合并
来源：http://hz.cdnleiting.top/gtagqxocch.html

Py:   ",".join(items)
来源：http://hz.kuanghao11.cn/gtcfrimivd.html

PHP:  implode(",", $items);
来源：http://hz.jqgufenzy.top/gtmmocnook.html

JS:   items.join(",")
来源：http://hz.wangdashe.top/gtujpnrbsd.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtjzysaucc.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtubbqfwld.html

Go:   strings.Join(items, ",")
来源：http://hz.dashuyun.cn/gtdyotjqwn.html

Ruby: items.join(",")
来源：http://hz.andypj.xyz/gtrdqmoukk.html

C#:   string.Join(",", items)
来源：http://hz.svipenyu.cn/gtoifydany.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtftzxlwzj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xziqi.cn/gtvhdmpmhp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangdashe.top/gtxvwutehc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtojvtgqph.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtortgsbyb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ydzc1.top/gtzeuxhlhg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xinyue.icu/gtludpgzul.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtxavcotne.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yanxiufei.cn/gttkubjgxt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.bjfxy.top/gtspbzbgvb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtccqguzlx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jiagoushi.top/gtljfwxcrd.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtkijxjeeq.html

TS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtvpmjwnnz.html

Java: String.format("%03d", 7)
来源：http://hz.hywenlv.cn/gtlruliwde.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgfzy.top/gtxusjauha.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtfawflbau.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sweek.top/gtdpirmbdl.html

[E11] 反转字符串
来源：http://hz.tianlin.xyz/gtdblxshlb.html

Py:   s[::-1]
来源：http://hz.316326.xyz/gtfhibrrjs.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtnjhbdefr.html

JS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtfbyfrpeq.html

TS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtlpjjaykj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuanzhike.top/gtmhlnrabt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gtkualuxcw.html

Ruby: s.reverse
来源：http://hz.hammf.cn/gthylmkvmm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtfflqnhfr.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtzyxnzvnd.html

Py:   s.count("a")
来源：http://hz.guannengcc.top/gtvdspdikn.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtcrnzpzvh.html

JS:   s.split("a").length - 1
来源：http://hz.cheryme.top/gtatdobtbm.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtevuhmjxt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.smart0.xyz/gtpyhvvfiz.html

Go:   strings.Count(s, "a")
来源：http://hz.316326.xyz/gtviyhouia.html

Ruby: s.count("a")
来源：http://hz.pycfn.com/gtvlabkfxi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gtxawgfhur.html

[E13] 逐字符遍历
来源：http://hz.jinghuilouyu.cn/gtpxwlggts.html

Py:   for ch in s: print(ch)
来源：http://hz.ywan-chungtsiang.top/gthbcblklw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xingfuxueyuan.xyz/gtbcipthzb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.meibo888.top/gtgdpzcgqc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtfejbhuvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gtjzowhaxj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtnxmkowqe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zdqjudy.top/gtcgjhzdgd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtdtoxkfjv.html

[E14] URL 编码与 Base64
来源：http://hz.aizwys.cn/gtqmlypdfn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cqqwz.cn/gtstjlalwg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhengqikj.top/gtjahamufa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangdashe.top/gtfjghupib.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gttmgvptdh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenlongwang.top/gtrlxjrupr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gtstgdyzcj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pengpengdd.cyou/gtdbqgebtm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yvedp.cn/gtuccrsabt.html

[E15] HTML 转义 / 反转义
来源：http://hz.cqqwz.cn/gtgolzxypb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.vqdsnc.cn/gtlemagcpf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtrohrjhin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cqqwz.cn/gtyzvusmzu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigufen.top/gtsuqnrpvd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guowangkeji.top/gtqueefcso.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtlpxiozpl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yangfankeji.com/gtnbrgnnhp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtrwmqvgpv.html

[E16] 数字千分位
来源：http://hz.zhaomingkeji.xyz/gtwiqiedpa.html

Py:   f"{1234567:,}"
来源：http://hz.sufxvd.cn/gtycajvonm.html

PHP:  number_format(1234567);
来源：http://hz.fzhhl.top/gtstidtlof.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zdqjudy.top/gtfflheahn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gthaurcvvc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xingfuxueyuan.xyz/gtpkerdcbq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gtzhowwnyy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gotoacloud.top/gtzvkbczdb.html

C#:   1234567.ToString("N0")
来源：http://hz.redwolf501.top/gtojoopxkx.html

[E17] 首字母大写
来源：http://hz.xziqi.cn/gtirwmqsqq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.9152youxi.cn/gtzqtsleel.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtrhtpfttz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtfrstjqwq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtyghrqkbi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sysykeji.top/gtgfedeiwb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgufenzy.top/gtafwrzwav.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtjdwhmkkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.smart0.xyz/gtpdmimnad.html

[E18] 模板占位符替换
来源：http://hz.aibaodan.cn/gtgpbzmmsl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.redwolf501.top/gtpdikkkju.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.52xcode.cn/gtxprizxpc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtzixaknol.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtcrbkirpl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sweek.top/gtfwmmwrjh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhongyouzk.top/gthqfainis.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dianchejie.cn/gtcuvrtebu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.birdmap.top/gtfybxkvdh.html

[E19] 多行文本按行拆分
来源：http://hz.hongshengwenyu.top/gtuebeiybz.html

Py:   s.splitlines()
来源：http://hz.sufxvd.cn/gtvbitytme.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.havefunace.top/gtscdgfnha.html

JS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtuyalaqnb.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtigjzesmr.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtkxvmvnia.html

Go:   strings.Split(s, "\n")
来源：http://hz.dianchejie.cn/gtnzygtkfb.html

Ruby: s.lines
来源：http://hz.c1oappe.top/gtgqcpwjmy.html

C#:   s.Split('\n')
来源：http://hz.shangyingyoupin.top/gtviaaerva.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtpfnrfatt.html

Py:   if not s:
来源：http://hz.daxiang520.top/gtxfkdzybk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtqyrluamy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cdnleiting.top/gthnobrnzi.html

TS:   if (s === "") {}
来源：http://hz.redwolf501.top/gtrcirdynn.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtblzadhom.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gtliqodzdn.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtivuvvopo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtcypqgdoi.html

[E21] 超长截断加省略号
来源：http://hz.feifeiyinyue.top/gtpnwhkcpn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj202588.top/gtznvfvtdz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ivvv.top/gtuvskbzrx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtronhmlfw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtcjgvpruq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtazdvjsfn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xinyue.icu/gtmpgugyhc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtsdyxanhx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gtbiiotmpv.html

[E22] 字节长度与字符长度
来源：http://hz.chenzaomai.com/gtjuuirohv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aizwys.cn/gtyjqculgd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gttsrjydgo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtbnshrmdd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtujnowocr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtfvgilbnq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtmadzdtev.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtweznclbk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gtrmsfcxde.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpevhjwcs.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtsfskdfhc.html

================================================================================
来源：http://hz.xuanzx.com/gtqnxayljz.html

[F01] 读取整个文件
来源：http://hz.daria6918.cn/gtenwzccqa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtpylsxlsu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jqgfzy.top/gtpcikgyqa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtdacduecv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gttkdnyfrl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtxtobluzt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hfpthk.cn/gtybjdypnc.html

Ruby: File.read("a.txt")
来源：http://hz.birdmap.top/gtvixjrgdo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sysykeji.top/gtriyziqmn.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtitkfktqn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtnxuenssa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuetiantiany.cn/gtmpxnoftr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtcisqudvb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtcmhwspol.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtezmkdvnb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gttbdasaxf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hongshengwenyu.top/gtzgprqerj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cqqwz.cn/gtwvykgrat.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigfzy.top/gtkrjuodpm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtpyhguirk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydzc1.top/gtcrerbvzi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtanhfwpvw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtmuwlocwu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gtyluepirt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydzc1.top/gtryrqsukn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtlfnmxdvn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtjolslzbt.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gtgozssrip.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gteysyvkdf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxuanxn.top/gtriowrlel.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtrbxoxwor.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtdqcwipiy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.svipenyu.cn/gthzeogmaw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtydzmimmq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtgoyqnfsn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuanzx.com/gtctngwday.html

[F05] 判断文件或目录是否存在
来源：http://hz.jianghu66.top/gtmrrulddc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.iojbl.cn/gtsetealke.html

PHP:  file_exists("a.txt");
来源：http://hz.zhoulong.xyz/gtsosjhfhl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtctpzusdv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtcjogslrx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtrwrhgbre.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guannengcc.top/gtezvycsaj.html

Ruby: File.exist?("a.txt")
来源：http://hz.316326.xyz/gtnervcbku.html

C#:   File.Exists("a.txt")
来源：http://hz.cdnleiting.top/gtfgxqkosg.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtccqilmoz.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258888.top/gtclzidlvd.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtahtnoacs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtjcocgjjd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtnubvidef.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtmrhespvb.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtwwwhohkk.html

Ruby: File.delete("a.txt")
来源：http://hz.snrcjt.cn/gteoyzbswg.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gttmuzzvqo.html

[F07] 创建目录（含多级）
来源：http://hz.zhaomingkeji.xyz/gtyutyfcqq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangkeji.top/gtztwjsuqw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gtdvftcdjg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtafqllnaw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtuoejsvas.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.iojbl.cn/gtmixvbzxt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.9152youxi.cn/gtoiwaesbb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gtdvjfvcng.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydzc1.top/gtlnviivqz.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtbysbmizs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtlgluqvgr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gtmkvueolh.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtvhgdzimg.html

TS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gttijqetxg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtoxhknfvf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ppjwa.cn/gtwjirpmzk.html

Ruby: Dir.children("dir")
来源：http://hz.fengsongda.top/gtkymzojys.html

C#:   Directory.GetFiles("dir")
来源：http://hz.haohaochexian.top/gtksjvwvef.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtiixuntmu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtmbumatkc.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gttjxdfsca.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtialbzqhr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtcrafbeyw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtvcrhncbm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hongshengwenyu.top/gtlocyuoqf.html

Ruby: File.size("a.txt")
来源：http://hz.ivvv.top/gtcsykduoq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinghuilouyu.cn/gtubysplei.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtfeiuskbb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtdcmcdktx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtrjpkkfta.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtgvqkbzwq.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gtptdzvfac.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jlsjyb.cn/gtzdrqfpwc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.meibo888.top/gtnyobafvq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtngvucnzj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuanzhike.top/gtpnwynfkp.html

[F11] 复制与移动文件
来源：http://hz.guowangkeji.top/gtgkjckoaq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtfcvnawql.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gtodurpmsl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtzltsjuew.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gteojvdiiy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gttypsmvai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jlsjyb.cn/gtybgzppgb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtggagysvb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jlsjyb.cn/gthfnfvorw.html

[F12] CSV 读写
来源：http://hz.jiagoushi.top/gtycnfvnik.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuanzhike.top/gtgcgpvnff.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.snrcjt.cn/gtffqaqsbd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxinkj.top/gtnaxxvazg.html

TS:   // 同上
来源：http://hz.sysykeji.top/gthkyzmblj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cashguo.top/gtohghidoo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtzaimujzq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sweek.top/gthwzzmver.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtufsikjdo.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkwbssgaz.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtewxzaopd.html

================================================================================
来源：http://hz.redwolf501.top/gtsnaqenqw.html

[G01] 定义类
来源：http://hz.kuanghao11.cn/gtkdsnmezl.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gtvucelxin.html

PHP:  class User {}
来源：http://hz.fzhhl.top/gtragiwqhj.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gtqqixxkyd.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtvvuhrscy.html

Java: class User {}
来源：http://hz.chenjidiqi.icu/gtgziodnjt.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gtwaswmhhv.html

Ruby: class User; end
来源：http://hz.gzhubu.top/gtftoxvlxp.html

C#:   class User {}
来源：http://hz.hnxiangtu.top/gtmgbhlifc.html

[G02] 构造函数
来源：http://hz.jiagoushi.top/gtiizmiprd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xinyue.icu/gthcwmvkdf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtcsrxbinc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtebguxomi.html

TS:   constructor(public name: string) {}
来源：http://hz.shzxlz.cn/gtcvrosqpz.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtkulsjwdv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtylkuuxep.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.haohaochexian.top/gtxysemzik.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtufixlhdd.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtascxhlmi.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtnsphhlej.html

PHP:  public string $name = "x";
来源：http://hz.chenzaomai.com/gtdnzkkktc.html

JS:   this.name = "x";
来源：http://hz.birdmap.top/gtugxecebu.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtggiaooqe.html

Java: private String name;
来源：http://hz.zhixingplan.top/gtnvtaflvm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigfzy.top/gtinjexzgw.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtxuszsvsy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtbdlpuyzh.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtyztawloc.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258.top/gtvsqnfpwn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtoefquqaq.html

JS:   greet() { return this.name; }
来源：http://hz.cucudq.cn/gtbpqltvtk.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtntbvbayy.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangtech.top/gttgtmouaw.html


<!-- 参考信息 -->