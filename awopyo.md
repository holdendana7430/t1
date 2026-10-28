代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.aizwys.cn/gtygmvsejy.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtyifdjeci.html

TS:   items.join(",")
来源：http://hz.dashuyun.cn/gtlxhkauyu.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gtmrlopulf.html

Go:   strings.Join(items, ",")
来源：http://hz.pengpengdd.cyou/gtodozvmuh.html

Ruby: items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtjoezbbyz.html

C#:   string.Join(",", items)
来源：http://hz.yonumen.top/gtsqoflsee.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtqxyfatgb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cucudq.cn/gthrmjiiso.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.smart0.xyz/gtikopnstd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gthuogxnhd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtnxieodpe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtitbjsfig.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.smart0.xyz/gtrduemkjr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daxiang520.top/gtlntzchiq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gtrezzlxmo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.aibaodan.cn/gtrnqpwvgd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.andypj.xyz/gtsckbueeq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtdeexkxrm.html

JS:   "7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtubukovts.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtpqvozkuz.html

Java: String.format("%03d", 7)
来源：http://hz.xinyue.icu/gtajrcpbot.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxuanxn.top/gtwzrfebjm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtkqojzwcn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aizwys.cn/gtilcqbwni.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtgockigar.html

Py:   s[::-1]
来源：http://hz.yanxiufei.cn/gtbubkevgk.html

PHP:  strrev($s);
来源：http://hz.zycfv.cn/gtirsqxufz.html

JS:   [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtrwkgqfis.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtbikaynzr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cqqwz.cn/gtwowmpzqo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gtfqzihocm.html

Ruby: s.reverse
来源：http://hz.zdqjudy.top/gtsmxnfxye.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtwrxjfwpk.html

[E12] 统计某字符出现次数
来源：http://hz.xuanzx.com/gtvhmkykbl.html

Py:   s.count("a")
来源：http://hz.xuetiantiany.cn/gtaooeicdj.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtnysxpnix.html

JS:   s.split("a").length - 1
来源：http://hz.cheryme.top/gtloqgvyif.html

TS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtzuzttwuj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.feifeiyinyue.top/gtqryvhxaf.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtbyjeqtzm.html

Ruby: s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtjfaxfljv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhijiandao.cn/gtycwcveav.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gtimxzztus.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtmmukxowz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guowangkeji.top/gtmfepvcni.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtfflwfzpu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtghxiwcvx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuanzx.com/gtebystwin.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtfjgqwiux.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtlvjoyrhf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.birdmap.top/gtvihvgpin.html

[E14] URL 编码与 Base64
来源：http://hz.zhixingplan.top/gtnpxayqlm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sweek.top/gtlnzazdjg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yanxiufei.cn/gtsuerajbs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ybcxt.top/gtkkaqdjma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.snrcjt.cn/gtculgxwyl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xziqi.cn/gtzzwjeusc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xinyue.icu/gtqfabxubz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuanzx.com/gtwcmzsirl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.feifeiyinyue.top/gtlaqujdcx.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigufen.top/gthyqmwafm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxuanxn.top/gtuysdapen.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtkncucinu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.havefunace.top/gtedcjmxjo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yonumen.top/gtxampraex.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cashguo.top/gtlnaxbfji.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.52xcode.cn/gtcoisqgex.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtoafiveru.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yonumen.top/gtgvkxcqki.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtaiudxavf.html

Py:   f"{1234567:,}"
来源：http://hz.hfpthk.cn/gtndmsihup.html

PHP:  number_format(1234567);
来源：http://hz.ydjk.org.cn/gthyhnrxij.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtrdeiihti.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtkbpehiib.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtjkdanutg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtofjxztrd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gttkdntjiu.html

C#:   1234567.ToString("N0")
来源：http://hz.snrcjt.cn/gtbqlbuicf.html

[E17] 首字母大写
来源：http://hz.shuidangran.top/gtzmsztfka.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cdnleiting.top/gtwvqueljb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ppjwa.cn/gtwwovugkx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gtqkxmkhan.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtvdzjoftp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gtnikpwumn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtcvbaotwt.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtktrdqqyx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.kuanghao11.cn/gtprhfilpu.html

[E18] 模板占位符替换
来源：http://hz.ywan-chungtsiang.top/gtkbutjzxz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gtbeljxtsg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtemyvkkks.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtxhntilbv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtibmjxguf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cucudq.cn/gttntgfnvz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj202588.top/gtlzffchqb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daxiang520.top/gtobllyogg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtrewpvfvf.html

[E19] 多行文本按行拆分
来源：http://hz.feifeiyinyue.top/gtdztezafd.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtagqpqiuo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gtxenornml.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtybrqfmrh.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtoxeogqhp.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtynmtwkuc.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gthtnzznoh.html

Ruby: s.lines
来源：http://hz.daxiang520.top/gtkfzvspgh.html

C#:   s.Split('\n')
来源：http://hz.9152youxi.cn/gtcpewjqtb.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtpmyejflk.html

Py:   if not s:
来源：http://hz.yj20258888.top/gtcpubcdzt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtfsrjneqr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cashguo.top/gtnmgaeqxv.html

TS:   if (s === "") {}
来源：http://hz.jinqigufen.top/gtjzzzxjzt.html

Java: if (s.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtwhdkiivs.html

Go:   if s == "" {}
来源：http://hz.jinyuanbaomall.cn/gtobsysvfo.html

Ruby: if s.empty?
来源：http://hz.jyoumei.cn/gttffomtak.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gtodkoewfs.html

[E21] 超长截断加省略号
来源：http://hz.hnqzz.top/gtygcadsce.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guowangkeji.top/gtdokonnec.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cucudq.cn/gtggfmlowq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtpjhktkti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtyettoqtu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtismnqxpo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gtfhtwrxlz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtldcuolby.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zdqjudy.top/gtancwudcd.html

[E22] 字节长度与字符长度
来源：http://hz.pengpengdd.cyou/gttowrjrjh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtncrmlvdx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtzpjnsmmm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtpljejjor.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtztwuqune.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hammf.cn/gtjwihdzkv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.iojbl.cn/gtefgaibhu.html

Ruby: s.bytesize;  s.length
来源：http://hz.tanke756.top/gtzonbfhqo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yueranfly.top/gthtnfjrjd.html

================================================================================
来源：http://hz.chenzaomai.com/gtcjwjkfiy.html

F. 文件与目录
来源：http://hz.jianghu66.top/gtaesliowl.html

================================================================================
来源：http://hz.gaohongyu789.top/gthgymiryd.html

[F01] 读取整个文件
来源：http://hz.9152youxi.cn/gtldyxofkg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dianchejie.cn/gtzaqcrhyh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shuidangran.top/gtnweviaka.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dianchejie.cn/gtfgwzlcdn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gtsrwpkpqd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtqnvglhgu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtypllmjcx.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtuasmrpbo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtoybxzdcj.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtokijwbvu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aibaodan.cn/gteojzimvu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtsfpurbla.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtfefdmcrk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtluxnxxvw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtravqzdbg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtprytqwyr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtotytkutr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtadkawlha.html

[F03] 写入文件（覆盖）
来源：http://hz.jyoumei.cn/gtjwezsxet.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dashuyun.cn/gtqtsbhweq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cucudq.cn/gtalpzzpcd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtumsgnucw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtmsfblmbm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtbufstiqr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yonumen.top/gtvmaobbgd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tianlin.xyz/gtxgqhwbeg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtimgnlxsi.html

[F04] 追加写入文件
来源：http://hz.0kj1m.cn/gtvejnmjyo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtsrwggjtv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xinyue.icu/gtkkjkomoj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtkseyserm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtxgilwsls.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fzhhl.top/gthrkhdfuq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.svipenyu.cn/gtoyvddiju.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.andypj.xyz/gtztgktwqs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydzc1.top/gtcbgcweak.html

[F05] 判断文件或目录是否存在
来源：http://hz.quarkkingdee.top/gthhhqvqhf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hfpthk.cn/gtjfqixbba.html

PHP:  file_exists("a.txt");
来源：http://hz.feifeiyinyue.top/gtzxiiwmce.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtelewobky.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtxgnhautk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtvwtcvayo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.vqdsnc.cn/gtfgqbsbti.html

Ruby: File.exist?("a.txt")
来源：http://hz.cdnleiting.top/gtvhljexqn.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gtoxzfsydm.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gthjcxqlrb.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtvgoqcayu.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gturtpbdkt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtudjjjgua.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtpwipgyro.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtjhrwejmx.html

Go:   os.Remove("a.txt")
来源：http://hz.ivvv.top/gtsubxogjv.html

Ruby: File.delete("a.txt")
来源：http://hz.kuanghao11.cn/gtprmfjwhn.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtnrmetfrw.html

[F07] 创建目录（含多级）
来源：http://hz.zycfv.cn/gtypjuupkq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxinkj.top/gtfoxhuvvd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.svipenyu.cn/gtjysspjaq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtqbtfytao.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gttbgfidzx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gtfkrlbsvs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gtzoxpkrbe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhengqikj.top/gtgwwevown.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtxsyacwtf.html

[F08] 遍历目录
来源：http://hz.zhaomingkeji.xyz/gtnschuaiq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.dianchejie.cn/gtzzhjxght.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtitcdsooz.html

JS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtchnrbaea.html

TS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtysbwqpux.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gteqlunisi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxinkj.top/gtopsnuhzu.html

Ruby: Dir.children("dir")
来源：http://hz.xylfe.cn/gtkazmxxki.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pengpengdd.cyou/gtonzzgrgk.html

[F09] 获取文件大小
来源：http://hz.tianlin.xyz/gtisewpfkj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dianchejie.cn/gtmxkutkol.html

PHP:  filesize("a.txt");
来源：http://hz.jqgfzy.top/gtirpjtcrk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtgoxwuzmw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtvhbmyokc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtnnxxbxqb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtwvthhehi.html

Ruby: File.size("a.txt")
来源：http://hz.aizwys.cn/gttlxcflek.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daria6918.cn/gtqptpcbcx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.snrcjt.cn/gtslyqjppn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtnyyijhvt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yangfankeji.com/gtabanxevz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtdhuxbawy.html

TS:   path.extname("a.txt")
来源：http://hz.bjfxy.top/gtqlcbrdnb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtyjxeyapp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtvlamszgx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtuxkrjvkp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dashuyun.cn/gtegyppvtp.html

[F11] 复制与移动文件
来源：http://hz.chenjidiqi.icu/gtsemiyedq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtxkmfpycc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sysykeji.top/gtzxnlczgs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtnjopcgan.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtddqugvki.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtwnaqfcxc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.quarkkingdee.top/gtuxlwvzeh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtrtlbrpjz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangdashe.top/gtflgoohsp.html

[F12] CSV 读写
来源：http://hz.shzxlz.cn/gtsanrpfly.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hfpthk.cn/gtwbupfyuj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gtsrkxdfke.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuanzhike.top/gtaqzubdcy.html

TS:   // 同上
来源：http://hz.xingfuxueyuan.xyz/gtaaytmitp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hammf.cn/gtelmnsibp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangdashe.top/gtmrsmagoq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtwixswmqm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhoulong.xyz/gtwzpzhlhu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtubuenfnr.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtletncrwh.html

================================================================================
来源：http://hz.yj202588.top/gtbzgsrtjk.html

[G01] 定义类
来源：http://hz.iojbl.cn/gtuwbcfjwr.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtvnseluxg.html

PHP:  class User {}
来源：http://hz.sufxvd.cn/gtcqzaxvee.html

JS:   class User {}
来源：http://hz.ydjk.org.cn/gtsprwstln.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtrgmtquqr.html

Java: class User {}
来源：http://hz.316326.xyz/gtrdhobgxg.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtychdxzuh.html

Ruby: class User; end
来源：http://hz.yuxming.cn/gtmbaugiuz.html

C#:   class User {}
来源：http://hz.yuanzhike.top/gtttrwkzrq.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gtcaqhnlyx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtnlihnigk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtjpuexxnl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtohcskywm.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtklynzsha.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtjozrcxkt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhoulong.xyz/gtlggdiaqn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtrxpvfywz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydzc1.top/gtyryozsos.html

[G03] 实例属性
来源：http://hz.cheryme.top/gtavmueuom.html

Py:   self.name = "x"
来源：http://hz.zhijiandao.cn/gtmazxkgmd.html

PHP:  public string $name = "x";
来源：http://hz.fzhhl.top/gtmsjkcpyb.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtsxurfncq.html

TS:   name: string = "x";
来源：http://hz.zhongyouzk.top/gtfjxihjam.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtevmxjqox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gtteipzbds.html

Ruby: @name = "x"
来源：http://hz.zdqjudy.top/gtjycqzfux.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtlhscculf.html

[G04] 定义方法
来源：http://hz.chenzaomai.com/gtfdfbanyd.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtfdlyzicg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj202588.top/gthoxvpikw.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtrttdhpln.html

TS:   greet(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtxkkzivvl.html

Java: String greet() { return name; }
来源：http://hz.havefunace.top/gtqkmdqbrv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yonumen.top/gtuaplcxet.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtxzjbuoyr.html

C#:   public string Greet() => Name;
来源：http://hz.hfpthk.cn/gtjdgygvjo.html

[G05] 继承
来源：http://hz.andypj.xyz/gtuumcreyp.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtsxopieip.html

PHP:  class Admin extends User {}
来源：http://hz.ppjwa.cn/gtirodcojb.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gttuvnumwg.html

TS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtugfxyddq.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtscugxrry.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yueranfly.top/gtbonxphkc.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gtigsuczbb.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtrqxqmxmy.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtngyokokp.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtrdbdnpwj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtzqvjyydq.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtonqelxnt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtqwnmhlgl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtrrojigyv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtzpkoqmcw.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtiekvkizd.html


<!-- 参考信息 -->