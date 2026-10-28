代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yanxiufei.cn/gtdyxnffai.html

TS:   s.split(",")
来源：http://hz.jinqigfzy.top/gtqppgmiql.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangshuangyany.cn/gtpqqhfqvn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhixingplan.top/gtfoasnpig.html

Ruby: s.split(",");  s.split
来源：http://hz.quarkkingdee.top/gtybzvwoed.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xingfuxueyuan.xyz/gtzasqtpfl.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258888.top/gtldmaoaaa.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtbughegvv.html

PHP:  implode(",", $items);
来源：http://hz.xuetiantiany.cn/gtofjgvskg.html

JS:   items.join(",")
来源：http://hz.bjfxy.top/gtsatfsyra.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtwslgsjrl.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtzhrphzvb.html

Go:   strings.Join(items, ",")
来源：http://hz.yuxming.cn/gtrunvgtap.html

Ruby: items.join(",")
来源：http://hz.xuetiantiany.cn/gtnynfnnwd.html

C#:   string.Join(",", items)
来源：http://hz.aizwys.cn/gtbaedbeqr.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtqkzyrytp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gogol.net.cn/gtjsgxgqkz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cashguo.top/gtqxoefbje.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtinlgcojb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtqivexirm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhongyouzk.top/gtakoqdklz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fengsongda.top/gtrwrkrikf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtptzgoixx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydzc1.top/gtjooxldkf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xingfuxueyuan.xyz/gtbwbgsssl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjfxy.top/gtkbupxjbw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gttydsbrlh.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gthhqontqs.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtoesnjxes.html

Java: String.format("%03d", 7)
来源：http://hz.daria6918.cn/gtvzjprimr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtgkviafep.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtmchqzchx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gtyehrvxtv.html

[E11] 反转字符串
来源：http://hz.smart0.xyz/gtcgwenocb.html

Py:   s[::-1]
来源：http://hz.kuanghao11.cn/gtphelkwjn.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtshozkjcj.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gthqydgndt.html

TS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtjzbjsieg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtuhtsnxfj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinghuilouyu.cn/gtgzeumeam.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtvfqmwcyq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtzfaqrdac.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtaueqoeuf.html

Py:   s.count("a")
来源：http://hz.cucudq.cn/gthleoaond.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gtsnshhzye.html

JS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtcxftsblh.html

TS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gtlpnohpgg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.snrcjt.cn/gtolnvyfhy.html

Go:   strings.Count(s, "a")
来源：http://hz.daxiang520.top/gthybkpwiq.html

Ruby: s.count("a")
来源：http://hz.wangshuangyany.cn/gtclptqbgw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.smart0.xyz/gtgrfvfkfg.html

[E13] 逐字符遍历
来源：http://hz.zycfv.cn/gtuqdujbiy.html

Py:   for ch in s: print(ch)
来源：http://hz.hywenlv.cn/gtasitdcie.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sysykeji.top/gtfpcrsliq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtxnqdgfqo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtbtwqpofj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gtnrmaeamb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hywenlv.cn/gttikmgakz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daxiang520.top/gtxtyzbyvt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sysykeji.top/gtaidfvuxn.html

[E14] URL 编码与 Base64
来源：http://hz.cqqwz.cn/gtxxpivfgz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.mhx1999.top/gtwmteezti.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gtnkoqjdwf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtaabrrzli.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.smart0.xyz/gtkxlsqjua.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258888.top/gtngiepmhq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtrscofhdw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aibaodan.cn/gtdqlfcdkq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zdqjudy.top/gtcpaltlto.html

[E15] HTML 转义 / 反转义
来源：http://hz.yongpay.top/gtehobrfpn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtbnaopyqk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sufxvd.cn/gtgwzvholt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuetiantiany.cn/gtadabmdhp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aizwys.cn/gtftaredbn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xziqi.cn/gtlcyrzcle.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigufen.top/gtimmlbplu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xylfe.cn/gtqenedopr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtgdxmakbg.html

[E16] 数字千分位
来源：http://hz.xuanzx.com/gtpbncakvh.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtdikgepel.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtkurklkgt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtkaleqjvm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtuipfaals.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jlsjyb.cn/gtnpnlgdnt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtegdozyya.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gtdrnucxyc.html

C#:   1234567.ToString("N0")
来源：http://hz.hnxiangtu.top/gtutcfplyi.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtnefogjbe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtfftlpttm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hysaishi.cn/gthpztrvjq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gtfrdvlyza.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtuhjbdrpb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dashuyun.cn/gtghpoirqq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ywan-chungtsiang.top/gtqmvlmnym.html

Ruby: s.capitalize
来源：http://hz.zhijiandao.cn/gtnbqwyzvb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yonumen.top/gtmyxgmwyd.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtjsoalyxz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cqqwz.cn/gtjfvbmgrv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gthbgvhghp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtopaoilyd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtmqfvokcq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gteroybvyo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gtjzohojmp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydjk.org.cn/gtmrfonfbr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenlongwang.top/gtgmtxgqml.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtguuhpyim.html

Py:   s.splitlines()
来源：http://hz.sxryk.cn/gtseduprrk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtpgwgaoex.html

JS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtmkealdgp.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtchupwlfs.html

Java: s.lines().toList()
来源：http://hz.xuetiantiany.cn/gtfkdjermg.html

Go:   strings.Split(s, "\n")
来源：http://hz.dianchejie.cn/gtxgpcycln.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtwfetzkcl.html

C#:   s.Split('\n')
来源：http://hz.daxiang520.top/gtxazaqoka.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangkeji.top/gthgpipwaa.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gtiizpqirs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jyoumei.cn/gtnmxetxmp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.iojbl.cn/gtvwfbfptl.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtwdrymakc.html

Java: if (s.isEmpty()) {}
来源：http://hz.mhx1999.top/gtzmodrqry.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangkeji.top/gtomeaeaoi.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtcdoyddam.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gaohongyu789.top/gtjjyzvycb.html

[E21] 超长截断加省略号
来源：http://hz.52xcode.cn/gtsfkogsea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hywenlv.cn/gtfblbdvbv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shuidangran.top/gtetkroxwj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtctsobruk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtovexwryn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtdihjhrjd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jianghu66.top/gtjpqvhkfk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuanzhike.top/gtwvggygmw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydzc1.top/gtrgafkpms.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtoeouzvfm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hysaishi.cn/gtepjurbll.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtymyifepk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gotoacloud.top/gtsfiqfgig.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtldsrpery.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gtxcjkfxvy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ydzc1.top/gtwwwewdza.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtugcugzxf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.vqdsnc.cn/gtvieodfbp.html

================================================================================
来源：http://hz.daria6918.cn/gtrasqajue.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtqcsluvao.html

================================================================================
来源：http://hz.bjfxy.top/gtwfvavswe.html

[F01] 读取整个文件
来源：http://hz.xylfe.cn/gtajleliek.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtkjujqxpu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtrbmwlaas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinghuilouyu.cn/gtnnyyrinb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgufenzy.top/gtmjpqpbug.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtncbevvki.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ivvv.top/gtktylijym.html

Ruby: File.read("a.txt")
来源：http://hz.pycfn.com/gtcndsfxtw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jlsjyb.cn/gtfkufnynu.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtngzgkujj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhongyouzk.top/gtungbotva.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gtdbiytzei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtzeisjyas.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gthydsgnpt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtwdsywjzn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shangyingyoupin.top/gtozykqgkd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenjidiqi.icu/gtiefnhesn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.birdmap.top/gtnvcqzrle.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtimhaywin.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zdqjudy.top/gtevclsrwr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtihkwkvka.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtevvhcfoa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtugcfetcu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.vqdsnc.cn/gtwlfnxzbb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gtgqnvzrwk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ivvv.top/gtqiujgxhg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtxzuvozna.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtwedpubrn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gtanwbglqu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xylfe.cn/gtefjprzub.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtpqujzqdj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtzxrjfhum.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gtzcozwdvc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gtowqmfske.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhiwuduotai.top/gtexxahozu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cheryme.top/gtdioxkrri.html

[F05] 判断文件或目录是否存在
来源：http://hz.pengpengdd.cyou/gttmeuqsln.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtuvuofpzy.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtpfptqfhf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtoosjzakf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtfbdujgkx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtdpqegmzw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gtclpeesuu.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenlongwang.top/gtzopgryer.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtuoarcfby.html

[F06] 删除文件
来源：http://hz.feifeiyinyue.top/gtuborppwk.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gtvocvrmex.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtzvtorqwv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gttiewsubw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.andypj.xyz/gtuqkgjgfx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtguqgopid.html

Go:   os.Remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtenktwpaf.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtiqbpzopo.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtzcwztpyk.html

[F07] 创建目录（含多级）
来源：http://hz.xuetiantiany.cn/gtojdelyqy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.0kj1m.cn/gtejdaekvs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.smart0.xyz/gtmvpkfecl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtuisyssgs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtwzgzjaim.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.smart0.xyz/gtykkbwlji.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cashguo.top/gtsyefzsgu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtqrahqymd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtyzrxbjqh.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtvgjhbjfh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtvktpgvgg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ywan-chungtsiang.top/gtjpqclzdx.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtkmxmrncu.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtwnzcaioq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gttskpgmru.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.kuanghao11.cn/gtngszryhz.html

Ruby: Dir.children("dir")
来源：http://hz.tian-w.cn/gthyueylde.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtkydfviij.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtnsgrufrf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.52xcode.cn/gtgwqcmxio.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtowwpueuk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yonumen.top/gtvruycthg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtipjroxrk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtoatdfnmm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnqzz.top/gthzzocqzc.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gthzmmwndf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenlongwang.top/gtxochytzw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zycfv.cn/gtljchmlao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtepuntxam.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zycfv.cn/gtzfewgisy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtxtwtdvzj.html

TS:   path.extname("a.txt")
来源：http://hz.cheryme.top/gtxglldhyw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtxkwiewmv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yvedp.cn/gtdnkawzpo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtwhcgoyze.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtzhtiesxd.html

[F11] 复制与移动文件
来源：http://hz.fzhhl.top/gttwugvspr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtpkiteoch.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnxiangtu.top/gtbwozrhqk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtydviqbxi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtfqpwdkgr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtvyoplefu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sweek.top/gtidxfgnzp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtiysvoqek.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtzlovnsej.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtxddyrtvm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtigssohxn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenlongwang.top/gtrsvpycis.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gtjaxvdfir.html

TS:   // 同上
来源：http://hz.ivvv.top/gtggmhetvf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtzgmokitt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tian-w.cn/gttinroesw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtsrjhihgq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guannengcc.top/gtkipbdlae.html

================================================================================
来源：http://hz.jqgufenzy.top/gtsfiawxoc.html

G. 面向对象
来源：http://hz.wangshuangyany.cn/gtfcubqtob.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmekomjjm.html

[G01] 定义类
来源：http://hz.gogol.net.cn/gtgjhawnkn.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtoxvcslwl.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtuivzjngl.html

JS:   class User {}
来源：http://hz.jyoumei.cn/gtpafoigdq.html

TS:   class User { name: string = ""; }
来源：http://hz.iojbl.cn/gtqaoospet.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtamqjblgx.html

Go:   type User struct { Name string }
来源：http://hz.birdmap.top/gtbblzkraf.html

Ruby: class User; end
来源：http://hz.iojbl.cn/gtpuivthys.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gtdxqdfzvs.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtbahoqbyr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shangyingyoupin.top/gtkgatmotl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtsbgdduyz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtmyvekpqe.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtuanbbpde.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gthotqsgnl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigufen.top/gtufyqorfw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtuexynvsr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cdnleiting.top/gtmdftlhws.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtwmhtkpjw.html

Py:   self.name = "x"
来源：http://hz.ppjwa.cn/gtcxhvdjlt.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtiyrauowi.html

JS:   this.name = "x";
来源：http://hz.bjfxy.top/gtuwfpybed.html

TS:   name: string = "x";
来源：http://hz.ybcxt.top/gtzpckbupz.html

Java: private String name;
来源：http://hz.zycfv.cn/gttqcfastq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gtogpwdesd.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gthadzlurn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daxiang520.top/gtepfrmqoa.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtrdbeuril.html

Py:   def greet(self): return self.name
来源：http://hz.hongshengwenyu.top/gtsrtgioxp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtzhhklygs.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gteixnshjo.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtgccfufjn.html

Java: String greet() { return name; }
来源：http://hz.jinqigufen.top/gtrhiociby.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtkbocomjj.html

Ruby: def greet; @name; end
来源：http://hz.chenlongwang.top/gtafcgidxn.html

C#:   public string Greet() => Name;
来源：http://hz.guannengcc.top/gtgotbwsez.html

[G05] 继承
来源：http://hz.ivvv.top/gtfpolgjyx.html

Py:   class Admin(User): pass
来源：http://hz.cashguo.top/gtrvpqggxj.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtizecyzhx.html

JS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtlpjwhdgr.html

TS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtbkfiirpd.html

Java: class Admin extends User {}
来源：http://hz.dianchejie.cn/gtuicmkxnz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gtabkhyoms.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gticbyyoxb.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gtqtuzqfny.html


<!-- 参考信息 -->