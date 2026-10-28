代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtibpgstak.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtkdjhhnvh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigfzy.top/gtaginazio.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guannengcc.top/gtetpkzsku.html

C#:   s.Replace("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtgvjcmijh.html

[E07] 按分隔符拆分
来源：http://hz.52xcode.cn/gtwrmxytyo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zdqjudy.top/gttrrcfbik.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dianchejie.cn/gtliadlbws.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hfpthk.cn/gtbkjnogtr.html

TS:   s.split(",")
来源：http://hz.zhijiandao.cn/gtwcrtbacz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258888.top/gtztjgrrkv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xuetiantiany.cn/gteiwxelgc.html

Ruby: s.split(",");  s.split
来源：http://hz.birdmap.top/gtinziojsc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.9152youxi.cn/gtujfhxonp.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtywczooks.html

Py:   ",".join(items)
来源：http://hz.xuetiantiany.cn/gtkpsfxodc.html

PHP:  implode(",", $items);
来源：http://hz.snrcjt.cn/gtwsvwelsj.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtxldrlpth.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtcexfsncx.html

Java: String.join(",", items)
来源：http://hz.zhongyouzk.top/gteckzxnvi.html

Go:   strings.Join(items, ",")
来源：http://hz.yonumen.top/gttpgxzzxs.html

Ruby: items.join(",")
来源：http://hz.zdqjudy.top/gtlogptoiu.html

C#:   string.Join(",", items)
来源：http://hz.haohaochexian.top/gtmakguqbs.html

[E09] 去除所有空白字符
来源：http://hz.xziqi.cn/gtnahnyczx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jqgfzy.top/gtkyflseww.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhaomingkeji.xyz/gtcjkecaax.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xingfuxueyuan.xyz/gtydqgqdhw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtasrfdsqj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pycfn.com/gtqerhlsrm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtjmztpfza.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dianchejie.cn/gtorpednlw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtxwqiisgc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.wangdashe.top/gtegdcroqz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhongyouzk.top/gtojzkmnir.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yonumen.top/gthxgdfopv.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtjredwgiv.html

TS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtwrvuoevp.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtaodafslj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yangfankeji.com/gtylvcfxqo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtcstxpxfa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yuanzhike.top/gtwluirzop.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtkovmvggi.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtetpisnxc.html

PHP:  strrev($s);
来源：http://hz.birdmap.top/gtvifpnsrh.html

JS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtedcfoukm.html

TS:   [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtlysquria.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtdtebapfv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gotoacloud.top/gtlltkddbq.html

Ruby: s.reverse
来源：http://hz.ydzc1.top/gtlkeyhwix.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtartwwjhf.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gtlflixqgl.html

Py:   s.count("a")
来源：http://hz.shanyushiyangtech.top/gtgrolimvn.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gtbjskgexz.html

JS:   s.split("a").length - 1
来源：http://hz.hfpthk.cn/gtcgmblpiu.html

TS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtjxrfsufm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xziqi.cn/gtkjzchmcp.html

Go:   strings.Count(s, "a")
来源：http://hz.shangyingyoupin.top/gtynyfxxuu.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtmsyuvlcw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtuslsfihq.html

[E13] 逐字符遍历
来源：http://hz.ivvv.top/gtzrhzxidp.html

Py:   for ch in s: print(ch)
来源：http://hz.pengpengdd.cyou/gtwjqyctkp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtifvojhld.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gteiocxpbb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtdgaotowo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangshuangyany.cn/gtqpbiamtw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gogol.net.cn/gtseberyzw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xingfuxueyuan.xyz/gtcvrdmdgm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtlicawjsz.html

[E14] URL 编码与 Base64
来源：http://hz.cqqwz.cn/gtnbpjubxj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gtucniuzvg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.0kj1m.cn/gtoyboywuz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtxndcdyhn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtpzoyedgr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtpnzhblqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtkkzmyuck.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hammf.cn/gtslwvlaxc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xinyue.icu/gtdbafbgsh.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtzprbfsau.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtlpzzobou.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gaohongyu789.top/gtdusitfvu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtifkbkqii.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj202588.top/gtimuumujq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhixingplan.top/gtbpcdjyys.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daria6918.cn/gthquazopx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gtagqloteg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.feifeiyinyue.top/gtdtuydacx.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gtoikhaydp.html

Py:   f"{1234567:,}"
来源：http://hz.0kj1m.cn/gtrnouzkki.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtdvqqumii.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xingfuxueyuan.xyz/gtyiapbwge.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtmgcdumnu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ehwqpu.com/gtrzlhzvdp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtjmbysjiq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jianghu66.top/gtpxmwfnwp.html

C#:   1234567.ToString("N0")
来源：http://hz.yanxiufei.cn/gtooovayde.html

[E17] 首字母大写
来源：http://hz.xuetiantiany.cn/gtbmguiqdt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.c1oappe.top/gtprbhirnf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.bjfxy.top/gthlvxqzhv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hfpthk.cn/gteieoibbb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtjfhbzvca.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtuhmmzhmg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tian-w.cn/gtjojaihny.html

Ruby: s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtsfpwqgeq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.meibo888.top/gtpguloqjb.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangtech.top/gtrhdvnbkl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cucudq.cn/gtmxkseeae.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tanke756.top/gtleswmzzj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtfdopswlp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtsrzzjmog.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gtlzwzjhzn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuanzx.com/gtsrzkebyz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sufxvd.cn/gtdmwdrkbr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhiwuduotai.top/gtteeaislr.html

[E19] 多行文本按行拆分
来源：http://hz.jqgufenzy.top/gtyltayszi.html

Py:   s.splitlines()
来源：http://hz.yueranfly.top/gtxbeemppt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gthgjlcmfu.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtxkdjrjou.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtuybnnxok.html

Java: s.lines().toList()
来源：http://hz.yueranfly.top/gtfpecrxdl.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtebeahrsq.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtkpkvbbmg.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtxhzitsej.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtwxiwccae.html

Py:   if not s:
来源：http://hz.shanyushiyangtech.top/gtvoxfycol.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shangyingyoupin.top/gtjfntuviy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtvgzzraha.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gtkwudamef.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gttryblizg.html

Go:   if s == "" {}
来源：http://hz.zhijiandao.cn/gttqvywhgc.html

Ruby: if s.empty?
来源：http://hz.ydzc1.top/gtfvwmvgwf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.havefunace.top/gtrajtxczw.html

[E21] 超长截断加省略号
来源：http://hz.dashuyun.cn/gtfoiclecl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258888.top/gtpgfscfei.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtioclfjre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtuzzncxrb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtdpbmuxte.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtlatqcsfq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydjk.org.cn/gtqqybseeb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.svipenyu.cn/gtsbebvuyk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxinkj.top/gtpfpahwgy.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtvnzgdzor.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shzxlz.cn/gtvrsizxwh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtxafnenzn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gttwqhlyqp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtjxbycvuj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenzaomai.com/gtvnjvtbnh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhaomingkeji.xyz/gttbbztdxw.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gtxvhykokg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtqtpfigdo.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnnuphfzm.html

F. 文件与目录
来源：http://hz.yangfankeji.com/gtxsfkalmt.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnsppweex.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtjqbpupjg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.svipenyu.cn/gtebqstbrs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.vqdsnc.cn/gtvmxqeaqa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.snrcjt.cn/gttubbywki.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtoaxyzefl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtxhhlxgct.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtwjcaalsq.html

Ruby: File.read("a.txt")
来源：http://hz.meibo888.top/gtkelqmzct.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenlongwang.top/gtixgihlce.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gtrwzrvajy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cucudq.cn/gtjebfnjkd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj202588.top/gtserraobo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtxtbvzhlx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtjqgldtaw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtsphynnvt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgufenzy.top/gtlobzyzfu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daxiang520.top/gtjogcczlk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhengqikj.top/gtrfntdjyx.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtooekalwr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.andypj.xyz/gtxuuvjzyx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtjqiupmxw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtcogjamsq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtgogkbpkg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.havefunace.top/gtuxgxfxei.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ppjwa.cn/gtqhlredua.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtoxokoaeo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pycfn.com/gtmazujcwo.html

[F04] 追加写入文件
来源：http://hz.chenjidiqi.icu/gtufvzqjao.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shangyingyoupin.top/gtupwvxqkx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.wangshuangyany.cn/gtyqlfwrwi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtdwtyyzzn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtlxcvhdbu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zdqjudy.top/gtsqitnwnj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtkiyopnud.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sufxvd.cn/gtfbezgldx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sxryk.cn/gtefqvxqsm.html

[F05] 判断文件或目录是否存在
来源：http://hz.sweek.top/gtbjgwxgqp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gtdoaftusu.html

PHP:  file_exists("a.txt");
来源：http://hz.kuanghao11.cn/gtomwtauav.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtlgdpmtjr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtikxibglf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj202588.top/gthosrjvvg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxuanxn.top/gtpfrksczk.html

Ruby: File.exist?("a.txt")
来源：http://hz.nwbrower.top/gtfaxwnkdl.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtegsnukzt.html

[F06] 删除文件
来源：http://hz.fzhhl.top/gtgumwhnzf.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gtikixtleu.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtgwqydrsg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtabfbenyk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtcdkxgedn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtfijkhfvo.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gthzqyoabj.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtifwvfltb.html

C#:   File.Delete("a.txt");
来源：http://hz.cqqwz.cn/gterffkogj.html

[F07] 创建目录（含多级）
来源：http://hz.zhongyouzk.top/gtwertzlwv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtykbyjroa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenjidiqi.icu/gtrziqjtjo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtxpwscjih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtnmurbnyj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.9152youxi.cn/gtscwccecr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ivvv.top/gtwxozkwrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gtauseulhv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fengsongda.top/gtsvtxllee.html

[F08] 遍历目录
来源：http://hz.jlsjyb.cn/gtqrefcwcq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtrkslzdsx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gthxgpwxmx.html

JS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gteusqfyge.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtpzdxrfpk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yonumen.top/gtnvxpfiwf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtfieikasz.html

Ruby: Dir.children("dir")
来源：http://hz.sysykeji.top/gtmyxijqaa.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnqzz.top/gtxyqizpbt.html

[F09] 获取文件大小
来源：http://hz.jyoumei.cn/gtvhsawnms.html

Py:   os.path.getsize("a.txt")
来源：http://hz.c1oappe.top/gtbgldwyai.html

PHP:  filesize("a.txt");
来源：http://hz.ppjwa.cn/gtaltfxaih.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtbfezfewg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtmgslhldp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gttxlpgmqv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhongyouzk.top/gteiyfuirp.html

Ruby: File.size("a.txt")
来源：http://hz.gotoacloud.top/gtijmrgjkq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ehwqpu.com/gtegfuhvsf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtfzhygexg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gthnrwxbmw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenjidiqi.icu/gtureihsep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtdlpnlmoc.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtamzdjwrh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gtzvvcyhol.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cdnleiting.top/gtkqzbuhzo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtqjgvwioj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gthlyrmyyk.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtrjnzbode.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtbpgwugia.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtvyduliso.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtdanaaxen.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtlkqbuzsc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydzc1.top/gtgmzqchul.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtkyxfdnfr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtconwwqkr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtwhqewwtp.html

[F12] CSV 读写
来源：http://hz.snrcjt.cn/gtqzkzyasr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yvedp.cn/gtqdwcqtbg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtjqxourcc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangkeji.top/gtoovubbbo.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtmknhzftz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtitcmilng.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gaohongyu789.top/gtefgvgban.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtwabnquge.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtmrtagxmz.html

================================================================================
来源：http://hz.gotoacloud.top/gtlncxbeoc.html

G. 面向对象
来源：http://hz.guannengcc.top/gtaaefuurh.html

================================================================================
来源：http://hz.snrcjt.cn/gtvyaotrhm.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gthszwewlo.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtwememtrp.html

PHP:  class User {}
来源：http://hz.kuanghao11.cn/gtqvqrdcbj.html

JS:   class User {}
来源：http://hz.yongpay.top/gtehthirik.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigfzy.top/gtumlmqxcb.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtyenajbai.html

Go:   type User struct { Name string }
来源：http://hz.pycfn.com/gtntmfvemp.html

Ruby: class User; end
来源：http://hz.nanxinkj.top/gtgieohukd.html

C#:   class User {}
来源：http://hz.pengpengdd.cyou/gttcsdnhtd.html

[G02] 构造函数
来源：http://hz.zhengqikj.top/gtsfqygzkh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.redwolf501.top/gthqxcansr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtjammgyjn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangdashe.top/gtiucvninu.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtudeuxazp.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gtnqlvbple.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtjombpayi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fzhhl.top/gtjqaixwem.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtdwwojnpq.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtwzfdooov.html

Py:   self.name = "x"
来源：http://hz.ydjk.org.cn/gtecictxby.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtjovnsftj.html

JS:   this.name = "x";
来源：http://hz.ehwqpu.com/gtlecmjmsa.html

TS:   name: string = "x";
来源：http://hz.jinghuilouyu.cn/gtqljgdvsz.html

Java: private String name;
来源：http://hz.yanxiufei.cn/gtlekxnnqt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.haohaochexian.top/gtjdvqbjzl.html

Ruby: @name = "x"
来源：http://hz.aizwys.cn/gtmoyislzn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtfxfdjxsv.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtuvhoxxke.html

Py:   def greet(self): return self.name
来源：http://hz.zhixingplan.top/gtwtqscgue.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtdlmeshel.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gtqqhucfgc.html

TS:   greet(): string { return this.name; }
来源：http://hz.birdmap.top/gtcudyifvy.html

Java: String greet() { return name; }
来源：http://hz.havefunace.top/gtfsgdyljx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtoxqskcea.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtroosqmjc.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtxrielzfi.html

[G05] 继承
来源：http://hz.zhaomingkeji.xyz/gtmcmlqrgi.html


<!-- 参考信息 -->