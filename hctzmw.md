代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtzygqoahx.html

Ruby: items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gtyempqxtz.html

C#:   string.Join(",", items)
来源：http://hz.yangfankeji.com/gtktdfljvx.html

[E09] 去除所有空白字符
来源：http://hz.zdqjudy.top/gtbpbwdynl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenzaomai.com/gtkgrfrwko.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jlsjyb.cn/gtpjhbwmnl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtcvgnbkzw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtwxxblopu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtzowdgnxr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.haohaochexian.top/gtantfgrnj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxuanxn.top/gtgotukkyu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.quarkkingdee.top/gtypxnhndy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.iojbl.cn/gtxfrcdbxs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sysykeji.top/gtvavddnvr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtboqzxvfx.html

JS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtzozvfipy.html

TS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtlxjehrhh.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtttmmsare.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hammf.cn/gtvpndkbcf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gthjmfyzek.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sysykeji.top/gtbvrkmjnz.html

[E11] 反转字符串
来源：http://hz.gotoacloud.top/gtuyuyqiry.html

Py:   s[::-1]
来源：http://hz.cucudq.cn/gtpyvnyzhi.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtatzklawf.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtwurherfy.html

TS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtvuhazykf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gtorixgwrt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.birdmap.top/gtkwrbannc.html

Ruby: s.reverse
来源：http://hz.zdqjudy.top/gtdirnijqg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtcatnqqfd.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtpeswokye.html

Py:   s.count("a")
来源：http://hz.gaohongyu789.top/gtaejgbrhc.html

PHP:  substr_count($s, "a");
来源：http://hz.xuanzx.com/gtgflapjnh.html

JS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtyrmmvswi.html

TS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtprjdiufg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhongyouzk.top/gtcgrfwbro.html

Go:   strings.Count(s, "a")
来源：http://hz.hnqzz.top/gticvpijke.html

Ruby: s.count("a")
来源：http://hz.hysaishi.cn/gtiotzhodf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtcizbuvcg.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtirjtcenu.html

Py:   for ch in s: print(ch)
来源：http://hz.snrcjt.cn/gtqkuhphiw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigufen.top/gtgeledjob.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtdbmvylyi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtlrlhhtzr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gotoacloud.top/gtdbpaniuw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.snrcjt.cn/gtycaamccq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yonumen.top/gtiakfawen.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shuidangran.top/gtgjjdmuxd.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtriubyrpq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cqqwz.cn/gtvtlvtjhy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj202588.top/gtzfqmmxhb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jianghu66.top/gttlvgpssm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtfcpjrkwr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cqqwz.cn/gtuxnavrcv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangkeji.top/gtivuddvzt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jianghu66.top/gtjtcllloy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.haohaochexian.top/gtpdgcfpcq.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gtcwcqylhm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgufenzy.top/gturhvqqfs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.redwolf501.top/gtkhvqfpwe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.andypj.xyz/gtuydhnkyc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pycfn.com/gtthboyuav.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangshuangyany.cn/gtqwmsufpu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangshuangyany.cn/gthzmkpafy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hfpthk.cn/gtymdklmxk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhongyouzk.top/gtcbosfsfp.html

[E16] 数字千分位
来源：http://hz.yueranfly.top/gtmievqfzt.html

Py:   f"{1234567:,}"
来源：http://hz.daxiang520.top/gtcxqefocj.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtnxphjxoy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gttycnkelw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtbubzxksy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jlsjyb.cn/gtcupchjqv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtwmfiwmxt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zdqjudy.top/gtvprgkjor.html

C#:   1234567.ToString("N0")
来源：http://hz.chenzaomai.com/gttftojccq.html

[E17] 首字母大写
来源：http://hz.daria6918.cn/gtxcqyjecz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhijiandao.cn/gtwubdbpdn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtewxthtpo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.0kj1m.cn/gtpyfsiklo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gthlwbomsx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gtdfftngpc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tanke756.top/gtzfhupqnw.html

Ruby: s.capitalize
来源：http://hz.0kj1m.cn/gtdpzwgpsz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cdnleiting.top/gthhkmtmvi.html

[E18] 模板占位符替换
来源：http://hz.pycfn.com/gtbxmzuneb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.iojbl.cn/gtqfcxslrj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xylfe.cn/gtbytbupgw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gttdgkwnuf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtiazzrpah.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtpcycgjtg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aibaodan.cn/gthsklqtqp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtkcxiktuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.svipenyu.cn/gtycvoemyn.html

[E19] 多行文本按行拆分
来源：http://hz.zhongyouzk.top/gtpljzhgrs.html

Py:   s.splitlines()
来源：http://hz.svipenyu.cn/gtzozwaugs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.smart0.xyz/gtlhpnwhly.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangtech.top/gtaahaoykh.html

TS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtmrstlklw.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtcjidxwyf.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangdashe.top/gtwnodadjz.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtrkvqplyp.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gttozxiias.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gtdhsjtvcn.html

Py:   if not s:
来源：http://hz.shanyushiyangtech.top/gtkrkqlods.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhijiandao.cn/gtslzenpeb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigfzy.top/gtfboixvge.html

TS:   if (s === "") {}
来源：http://hz.chenzaomai.com/gtqlzdubqf.html

Java: if (s.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtaqdsntcy.html

Go:   if s == "" {}
来源：http://hz.fengsongda.top/gtcycvlqfi.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtkrrbkqao.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhengqikj.top/gtxfgdgbej.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtclxahqbw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtcqqbqkjr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtveekipje.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtxgbhzgyw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtqqkvwbvk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtbxvnjclq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.redwolf501.top/gtknkaizla.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgfzy.top/gtamcloynt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yonumen.top/gtluhgdoij.html

[E22] 字节长度与字符长度
来源：http://hz.chenjidiqi.icu/gtlammxsca.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgfzy.top/gtznztzmbk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gthzwjngsn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtpdinqodi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtbrxfolkp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xinyue.icu/gtmtnkzoxb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.0kj1m.cn/gtkwpyvmys.html

Ruby: s.bytesize;  s.length
来源：http://hz.ehwqpu.com/gtfbyejkoq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pengpengdd.cyou/gtnobgersq.html

================================================================================
来源：http://hz.52xcode.cn/gtffsgenkf.html

F. 文件与目录
来源：http://hz.fzhhl.top/gtquypyjwm.html

================================================================================
来源：http://hz.daxiang520.top/gtbmurdjjl.html

[F01] 读取整个文件
来源：http://hz.zdqjudy.top/gthsrttfnp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtvylcrhbj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtjonmmmbl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hysaishi.cn/gtffpbrspn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.aibaodan.cn/gtwaevcxun.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtomiwxbdy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guowangkeji.top/gtsfmeqwsc.html

Ruby: File.read("a.txt")
来源：http://hz.shangyingyoupin.top/gtgzvsedvi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtodovsemn.html

[F02] 逐行读取文件
来源：http://hz.c1oappe.top/gtdjhjligk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtlaixmhbh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtxfcpqrnw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtuxwdmigr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtsvxathln.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtdtzksxqk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtdgewtsho.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jlsjyb.cn/gtsnmopizj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jyoumei.cn/gtqzqhnzer.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtzhapeuxe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtzcklltwy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aizwys.cn/gtqzuzmdxs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtyxbmices.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtfezesene.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenlongwang.top/gtvofkdkrj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gtvoqhtbhw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtjastpvzg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtrsnoeynz.html

[F04] 追加写入文件
来源：http://hz.wangdashe.top/gtounxeptr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.snrcjt.cn/gtuoinmppx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hysaishi.cn/gtzlldqjyy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtthbqypkw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtxipxysab.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gttuosrgix.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yanxiufei.cn/gtzbkmrdye.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnqzz.top/gtbreidmug.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtpvfaakqe.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinghuilouyu.cn/gtnpxmywmv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhoulong.xyz/gtktnnhpow.html

PHP:  file_exists("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtrverhmyb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtzmkeyfdm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtnplymdhh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtazviuyya.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtaspyqods.html

Ruby: File.exist?("a.txt")
来源：http://hz.bjfxy.top/gtdlqbbwqo.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxinkj.top/gtnasfursi.html

[F06] 删除文件
来源：http://hz.havefunace.top/gtasynmfer.html

Py:   os.remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtuzfbedcj.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gttxvtlhvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtddtyagms.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtgiiysifp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtphzixnxa.html

Go:   os.Remove("a.txt")
来源：http://hz.xinyue.icu/gtohxbwciv.html

Ruby: File.delete("a.txt")
来源：http://hz.yuxming.cn/gtxiujnkyf.html

C#:   File.Delete("a.txt");
来源：http://hz.guowangkeji.top/gtggspoaov.html

[F07] 创建目录（含多级）
来源：http://hz.nanxuanxn.top/gtbxpsotly.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ivvv.top/gtwhtyfupr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yanxiufei.cn/gtcbclnkqh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtovyfclfg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gthdxpqbna.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangkeji.top/gtlboodudt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtlbdtsoyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydzc1.top/gtdkxyqyqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtftmqiflg.html

[F08] 遍历目录
来源：http://hz.nanxinkj.top/gtmoyiqxvk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhaomingkeji.xyz/gtyrttzviy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cheryme.top/gtiwdtyeve.html

JS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtibrfqszp.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gthstrizqc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tianlin.xyz/gtgsywmwcc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gttnovtcmi.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtbycuomoc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtmtvcmtqf.html

[F09] 获取文件大小
来源：http://hz.yj20258.top/gtfncjluzn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gtllolejiu.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtbhgjntsk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtvigwqhbj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtutmkowut.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtadgvqlze.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xingfuxueyuan.xyz/gtcdjzmhbr.html

Ruby: File.size("a.txt")
来源：http://hz.hammf.cn/gtkbesydvv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtstslplxr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gttdfypbbn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtmodjyapr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shuidangran.top/gtmhabrnqo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtvurlppuz.html

TS:   path.extname("a.txt")
来源：http://hz.zhoulong.xyz/gtzxjmtrgi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.birdmap.top/gtzorlrgjb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hywenlv.cn/gtqijfbtpf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtcngotboj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tanke756.top/gtfofduwon.html

[F11] 复制与移动文件
来源：http://hz.pengpengdd.cyou/gtbbenhbjc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtmmaczmxd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtalfjszsq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtmuomhltu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtuzripdhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.meibo888.top/gtqhtztfmf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xylfe.cn/gtswkszjpf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtjifwrsgp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.vqdsnc.cn/gtzxfxaram.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtitznmrwe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cdnleiting.top/gtmzlqqehp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gtksbndtua.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gtoqtrnzxj.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtzvuvaddu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtjszuxkib.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yongpay.top/gtwgdavrsv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtnjpjniua.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fengsongda.top/gtefahigvy.html

================================================================================
来源：http://hz.xinyue.icu/gtlwgwtbkf.html

G. 面向对象
来源：http://hz.hywenlv.cn/gtfvlslygl.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtghxmkiqh.html

[G01] 定义类
来源：http://hz.jianghu66.top/gticmjkqpl.html

Py:   class User: pass
来源：http://hz.cqqwz.cn/gtsagesmkf.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtxiufyvzc.html

JS:   class User {}
来源：http://hz.hnxiangtu.top/gtrlodczvd.html

TS:   class User { name: string = ""; }
来源：http://hz.yueranfly.top/gtpwcrfaym.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtdrufyrbl.html

Go:   type User struct { Name string }
来源：http://hz.yj20258.top/gtdkdhjksa.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gtenuyvggs.html

C#:   class User {}
来源：http://hz.cucudq.cn/gtcfiywqxt.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtgpnerrrj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtaxirvhsx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnxiangtu.top/gtwvneuxmq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gttmdbdbjp.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangkeji.top/gtgwkpxdwe.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtrwzmdbyt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gtobrtwmli.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtvejhvprp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtzbtjnzap.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gtnthvnugp.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtxckzqcjl.html

PHP:  public string $name = "x";
来源：http://hz.pycfn.com/gtsvpkokah.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gthrjhztae.html

TS:   name: string = "x";
来源：http://hz.shuidangran.top/gtxopmgvgz.html

Java: private String name;
来源：http://hz.sweek.top/gtcccutoxd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gtvjzbbyqx.html

Ruby: @name = "x"
来源：http://hz.hfpthk.cn/gtdyuiqjpt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangdashe.top/gtuzcsiqdh.html

[G04] 定义方法
来源：http://hz.yj202588.top/gtiaetzmoi.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258.top/gtwclnknfz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtrnvdktnq.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtqplmjoen.html

TS:   greet(): string { return this.name; }
来源：http://hz.fengsongda.top/gtisnlfnmh.html

Java: String greet() { return name; }
来源：http://hz.aibaodan.cn/gtxujsqrtv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aizwys.cn/gtyxwgzgmr.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtkbeiyhio.html

C#:   public string Greet() => Name;
来源：http://hz.sweek.top/gtwysrgbvl.html

[G05] 继承
来源：http://hz.jqgfzy.top/gtlsuufhll.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtwycdqnvc.html

PHP:  class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtaltrosom.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtiftrsqaj.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gttxztdahd.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtwktqqxgf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtuobtuivp.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtyafskfiw.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gtrobdwxwx.html

[G06] 重写方法
来源：http://hz.daxiang520.top/gtmjcavdms.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtnlxnernj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtcijuumxm.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtnemoggmu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtrzolrjvz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtmjgbactp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.fengsongda.top/gtqovzcfyc.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtsxoyblkn.html

C#:   public override string Greet() => "admin";
来源：http://hz.316326.xyz/gtsnejfkwx.html

[G07] 调用父类方法
来源：http://hz.zdqjudy.top/gtobshblbm.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtzzzbuktn.html

PHP:  parent::greet();
来源：http://hz.iojbl.cn/gtjiqldwuw.html


<!-- 参考信息 -->