代发 wailian999

[E06] 替换子串
来源：http://hz.andypj.xyz/gtaxrdqvzx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guannengcc.top/gtvrkxhnya.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tian-w.cn/gtgbvbxrea.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtpfcpndsx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtkndmuywu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtglutpifx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnqzz.top/gtmoorcbhq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtvjhwunxz.html

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtwraennhb.html

[E07] 按分隔符拆分
来源：http://hz.ehwqpu.com/gtqlvpvknh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dashuyun.cn/gtxbharvgi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cashguo.top/gtrhksvhwy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydjk.org.cn/gtvukcarfl.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtdztqkypd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj202588.top/gtbpdvcdvv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shzxlz.cn/gtannjnhvx.html

Ruby: s.split(",");  s.split
来源：http://hz.zhaomingkeji.xyz/gtrxshsxfe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinghuilouyu.cn/gtpheovftc.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtoocfsoem.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtbfvssgly.html

PHP:  implode(",", $items);
来源：http://hz.9152youxi.cn/gtapjuassn.html

JS:   items.join(",")
来源：http://hz.9152youxi.cn/gtamqaxvwu.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtftrnbdsb.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtqqbipoll.html

Go:   strings.Join(items, ",")
来源：http://hz.sweek.top/gtugrlngaw.html

Ruby: items.join(",")
来源：http://hz.jinqigfzy.top/gtxwilqqlb.html

C#:   string.Join(",", items)
来源：http://hz.gaohongyu789.top/gtjyfewkiv.html

[E09] 去除所有空白字符
来源：http://hz.0kj1m.cn/gtzineazoh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.0kj1m.cn/gtpytcetix.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigfzy.top/gtqjdcmdtq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtjirvwhnu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtjoduugqw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtponhulqk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.vqdsnc.cn/gtehjqqufr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yonumen.top/gtzpnpaywm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yanxiufei.cn/gtgsklybkz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.wangdashe.top/gtavejandd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtfwhobtnn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hammf.cn/gtaarqvxwp.html

JS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtmvgjiarq.html

TS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtsjfzhbbx.html

Java: String.format("%03d", 7)
来源：http://hz.yuanzhike.top/gttslydxvm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yongpay.top/gtumypuxcc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.smart0.xyz/gteowqdarh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gtzajfzcey.html

[E11] 反转字符串
来源：http://hz.wangdashe.top/gtspvfrfxi.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtngfeiovd.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtouiefmta.html

JS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gterexanxq.html

TS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtlrgbyivy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ivvv.top/gtucezyrxv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.52xcode.cn/gtjufodhdj.html

Ruby: s.reverse
来源：http://hz.jqgufenzy.top/gtvjnievgn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtftfjuirr.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtkyowrouq.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gtfhygrfeb.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtvepcljre.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtoxpjeose.html

TS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtxbopmnbn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shanyushiyangkeji.top/gtwrnkcung.html

Go:   strings.Count(s, "a")
来源：http://hz.chenjidiqi.icu/gtmfmistay.html

Ruby: s.count("a")
来源：http://hz.haohaochexian.top/gtphwrsyud.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtrnsslyun.html

[E13] 逐字符遍历
来源：http://hz.tianlin.xyz/gtnfvgvvqi.html

Py:   for ch in s: print(ch)
来源：http://hz.hammf.cn/gtrpruozsw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daria6918.cn/gtmiyearrx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtlaotzsua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtormcstvg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.vqdsnc.cn/gtybacxiee.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangkeji.top/gtshkzvzmp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guowangkeji.top/gttcimiedq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xinyue.icu/gtbuimckxc.html

[E14] URL 编码与 Base64
来源：http://hz.cdnleiting.top/gtdavxyvrb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zdqjudy.top/gtyfybdred.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.redwolf501.top/gtetvgzrbw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hfpthk.cn/gthfulvqjs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.havefunace.top/gtpnrpgfqz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtjjexqpuy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhoulong.xyz/gtjxomppzd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtcqlcxlhp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtigctuzel.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtjpqiwywq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhoulong.xyz/gtyhezerbn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jyoumei.cn/gtnxlsusgr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gthfjlwttl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cheryme.top/gtnmwcoeoo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gtyfvnvdgf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nwbrower.top/gtuftojoes.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj202588.top/gtvvhrmgjm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.birdmap.top/gthjydfwec.html

[E16] 数字千分位
来源：http://hz.hnqzz.top/gtgjfufccg.html

Py:   f"{1234567:,}"
来源：http://hz.fzhhl.top/gtncmmbksg.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtqqsjivoo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtiqerurlk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtnevazffi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aizwys.cn/gtuxwjzssq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zdqjudy.top/gtaakixdge.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtxctejhjh.html

C#:   1234567.ToString("N0")
来源：http://hz.tanke756.top/gtncjzhfio.html

[E17] 首字母大写
来源：http://hz.jinyuanbaomall.cn/gtjjuoyfry.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sufxvd.cn/gtmzqcccxe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.kuanghao11.cn/gtiijsyhfi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gthuszbrvp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtywswkwxl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xinyue.icu/gtknqmlnys.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gtovisrjok.html

Ruby: s.capitalize
来源：http://hz.gzhubu.top/gtixclspow.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtubfrxlnm.html

[E18] 模板占位符替换
来源：http://hz.mhx1999.top/gttamxomte.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cucudq.cn/gtcbutercq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtahmolclc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gtrspurvzi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtbwavllol.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtbspftqhx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgufenzy.top/gtmlldsefk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jlsjyb.cn/gtvqakchyh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtkgkkpljh.html

[E19] 多行文本按行拆分
来源：http://hz.meibo888.top/gtkgrbsukt.html

Py:   s.splitlines()
来源：http://hz.sufxvd.cn/gtcryfzznh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gtiokfjbmz.html

JS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtjfwxpjpy.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtpunlhypd.html

Java: s.lines().toList()
来源：http://hz.guowangkeji.top/gtdazlqdzx.html

Go:   strings.Split(s, "\n")
来源：http://hz.hongshengwenyu.top/gtmcmajeqz.html

Ruby: s.lines
来源：http://hz.0kj1m.cn/gtkutlcxyy.html

C#:   s.Split('\n')
来源：http://hz.zhijiandao.cn/gthkdvyaqp.html

[E20] 判断字符串是否为空
来源：http://hz.ybcxt.top/gtlpxpnkmd.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtqomzmbnz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gotoacloud.top/gtzqlnfeyn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtiqqsledf.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gtmwtpodyw.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtzyvmciqb.html

Go:   if s == "" {}
来源：http://hz.birdmap.top/gtgfyhnqgw.html

Ruby: if s.empty?
来源：http://hz.zhixingplan.top/gtefloplbd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gtcjuxcctp.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gttmxsmlhf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.snrcjt.cn/gtuowgyfch.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenjidiqi.icu/gtsptvklaq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtrevpdnuy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtxfvvfdpz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtwvjkbcbk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtoaoxfpfl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtfloaachy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtxxdalqfy.html

[E22] 字节长度与字符长度
来源：http://hz.gotoacloud.top/gtsxmqrhsc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gtaztwypdj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtlvajizpt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtaswqjmhq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtautpgzon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtyrziljvx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.birdmap.top/gttypatfxv.html

Ruby: s.bytesize;  s.length
来源：http://hz.gzhubu.top/gtzjixqook.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ehwqpu.com/gtrwjdtdnb.html

================================================================================
来源：http://hz.guowangkeji.top/gtvsxmoeqt.html

F. 文件与目录
来源：http://hz.gzhubu.top/gttiaqsnqw.html

================================================================================
来源：http://hz.cashguo.top/gtqureymhw.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtdtqzujbt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtxsdxtkwi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xylfe.cn/gtngjxtwom.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtglasjakj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtxbyohcyq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtnlflubsj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shangyingyoupin.top/gtvmimqqdx.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtmaxfhaoy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtapohzjyd.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gtwpplaidc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.haohaochexian.top/gtfdysmcrz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gthtrahuxy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtvrjarjoa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtbpksvfqt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtwpnexbfv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtrtvktrdt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.feifeiyinyue.top/gtiwjammyc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgufenzy.top/gtaqlkadmc.html

[F03] 写入文件（覆盖）
来源：http://hz.sysykeji.top/gtknmfnahn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cdnleiting.top/gtxknjvenq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtyrjveyej.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtaiofuwvm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtgmzycbwc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxuanxn.top/gtvkevjscs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinyuanbaomall.cn/gtastzlpec.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtvmhstwca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cashguo.top/gtfhfikxgh.html

[F04] 追加写入文件
来源：http://hz.jinqigfzy.top/gtbgwfqiof.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.havefunace.top/gtldjfwvhs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtewlbemdv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtutvheakm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtrmtbbsat.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ehwqpu.com/gtfpbhfjmu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnqzz.top/gtrsyjhtqb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtdukhufle.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shuidangran.top/gttpwnhhqa.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gtdtkaosuj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jianghu66.top/gtljtwhxby.html

PHP:  file_exists("a.txt");
来源：http://hz.hnqzz.top/gtdumiqfxk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtdbbvtyvs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtlahjwinx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gttdevvcqz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gteropwgjs.html

Ruby: File.exist?("a.txt")
来源：http://hz.yvedp.cn/gtawdvlwbs.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtgdeeqlcl.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtwhlofqdq.html

Py:   os.remove("a.txt")
来源：http://hz.ppjwa.cn/gtytexxcyn.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtmejanseq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtjccawhlx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtgrdeaiqu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtlsdxeutd.html

Go:   os.Remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtehyeinvk.html

Ruby: File.delete("a.txt")
来源：http://hz.daria6918.cn/gthsqwelvc.html

C#:   File.Delete("a.txt");
来源：http://hz.sweek.top/gtrsjuoult.html

[F07] 创建目录（含多级）
来源：http://hz.zhiwuduotai.top/gteropmqnk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258.top/gtbuettivs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gzhubu.top/gtwlwljmio.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtncezhesq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtlzeexryl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gtuyprfkqy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.0kj1m.cn/gtjtvwfpxn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gtieomtxec.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jlsjyb.cn/gtkxzqvdfr.html

[F08] 遍历目录
来源：http://hz.feifeiyinyue.top/gtgywrxqug.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtzyxnaalu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtukhdaxdi.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtcmdrcrxi.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gttqmeraep.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtrjlghkcp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.feifeiyinyue.top/gtgexohhwc.html

Ruby: Dir.children("dir")
来源：http://hz.hammf.cn/gtprwtedli.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtlowyfdzr.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtypeocuko.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtmycnkxfd.html

PHP:  filesize("a.txt");
来源：http://hz.snrcjt.cn/gtvsdymtav.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtwfpefjez.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtuybivmyp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtrpudrqgw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtlvhksron.html

Ruby: File.size("a.txt")
来源：http://hz.nanxinkj.top/gtzhvilttx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.andypj.xyz/gtltzmzlqv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fzhhl.top/gtiafyvtvr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtjcxcqmbv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtvihqmqsk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtjhmoukbh.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtytsyygsl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hammf.cn/gtwjrlhlgy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gthaktdsoq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtoyvulkmm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtltvjemnw.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gthbmnejeb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtzailtfib.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gtvzeqsycj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtlhivmjgt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtnjqkvysm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydjk.org.cn/gtmyjfifit.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daria6918.cn/gtiqjhparf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtzoinzdwg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.smart0.xyz/gtwzozjpmw.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtontsblxv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtaevzajcq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gtxyodvwvl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtmcblxsdp.html

TS:   // 同上
来源：http://hz.redwolf501.top/gterpzibfb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aizwys.cn/gthcbcroij.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtgkfjimqj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtigauzrwa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gtrsspiqoi.html

================================================================================
来源：http://hz.fzhhl.top/gtktpdpwrc.html

G. 面向对象
来源：http://hz.ivvv.top/gtfmdrpepf.html

================================================================================
来源：http://hz.wangdashe.top/gtbhdxrfjb.html

[G01] 定义类
来源：http://hz.nanxuanxn.top/gtoxmxyiqe.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtlomfwrsa.html

PHP:  class User {}
来源：http://hz.9152youxi.cn/gtsfdchltg.html

JS:   class User {}
来源：http://hz.hysaishi.cn/gtinrjdnsr.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gtgbxenlli.html

Java: class User {}
来源：http://hz.shuidangran.top/gtocgjpyao.html

Go:   type User struct { Name string }
来源：http://hz.gzhubu.top/gtrebwhjfk.html

Ruby: class User; end
来源：http://hz.jinyuanbaomall.cn/gtzzqzrkrr.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gtuuezrzmy.html

[G02] 构造函数
来源：http://hz.sysykeji.top/gtldgjdmxt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gthwrwrdhy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtfcklffvw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtyudplawe.html

TS:   constructor(public name: string) {}
来源：http://hz.fzhhl.top/gtchskocol.html

Java: User(String name) { this.name = name; }
来源：http://hz.smart0.xyz/gtllajrehl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aibaodan.cn/gtnszhubpv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ivvv.top/gtmbrbqpzp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtsakiawzn.html

[G03] 实例属性
来源：http://hz.jianghu66.top/gtfzgkknbm.html

Py:   self.name = "x"
来源：http://hz.gogol.net.cn/gtvggiigbk.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtcvqfaoec.html

JS:   this.name = "x";
来源：http://hz.ehwqpu.com/gtldhmizjx.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtojozzrnr.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtdnhpeelf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtwgffvydf.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gttlngzlpr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.feifeiyinyue.top/gtzrqbdkkj.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtdmlmfqxm.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gtbwnrqbnv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtpxvsztag.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtkiwxmppo.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258.top/gtxzldwnan.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtjlgtnpqa.html


<!-- 参考信息 -->