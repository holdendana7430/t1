代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gttryigxnf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtmenhhnyx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fengsongda.top/gtwmizawvd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtfwlmfrac.html

C#:   s.Replace("a", "b")
来源：http://hz.tanke756.top/gtamhspwxt.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtlheuvsba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gogol.net.cn/gtyzixlckb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxinkj.top/gtsvztsfgb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtfcdywkll.html

TS:   s.split(",")
来源：http://hz.0kj1m.cn/gtggzwfutw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.birdmap.top/gtpquihhok.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhaomingkeji.xyz/gtqeyewqcn.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gthoyxmsru.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yueranfly.top/gtnufttngu.html

[E08] 数组按分隔符合并
来源：http://hz.pengpengdd.cyou/gtwrjbfudx.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gttlvdugad.html

PHP:  implode(",", $items);
来源：http://hz.dashuyun.cn/gtamyodayx.html

JS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gttrqvvodi.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gtesfnissd.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtwhnaovfz.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtdymvjbfv.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangtech.top/gtegrcoans.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtzcdfdnfd.html

[E09] 去除所有空白字符
来源：http://hz.xingfuxueyuan.xyz/gtdcocigtm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gotoacloud.top/gttdbzbfcn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gtbxsuwzxa.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtgnfeqpel.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtbcodymrw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtthoxmsat.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daria6918.cn/gtmpjglcdg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hammf.cn/gtvjhyybfn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hammf.cn/gttemvbplg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jianghu66.top/gtngryyucg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhijiandao.cn/gtdmawphqk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtcpouaonb.html

JS:   "7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtvuvylwmh.html

TS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtgkianndb.html

Java: String.format("%03d", 7)
来源：http://hz.chenzaomai.com/gtcuovpjwd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtztkxpfuo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gtcbiuezkn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.andypj.xyz/gtqgdhliqd.html

[E11] 反转字符串
来源：http://hz.guowangkeji.top/gtvyujkfun.html

Py:   s[::-1]
来源：http://hz.ehwqpu.com/gtjqjrbwjd.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gthmzwpobp.html

JS:   [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtanfvjwnd.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtadhafvjg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gtaaojfbha.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cheryme.top/gtsvwgcjmc.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtdomnuvgp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtswwhopqq.html

[E12] 统计某字符出现次数
来源：http://hz.yanxiufei.cn/gtqdnrisax.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtoczwktvt.html

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gtxultmtwn.html

JS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtvpgxwjhx.html

TS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtgocvbjex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtnobgimer.html

Go:   strings.Count(s, "a")
来源：http://hz.c1oappe.top/gtiejrvhsv.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtekingnvd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258.top/gtgrqeicze.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gtbhqppqpz.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtuxxxjuwz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.birdmap.top/gtqznzupos.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtuacxxbym.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtuqzdgsce.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gtglcabdmu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtwbtgyecn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ehwqpu.com/gtiwuqbumz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtbsypnahd.html

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gtjqizqodk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhongyouzk.top/gtxkvodtjd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gtubyeevca.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sxryk.cn/gtuldouymu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.wangdashe.top/gtvoxsfzkj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hongshengwenyu.top/gtznuyvbdg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dashuyun.cn/gthonhsecs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgfzy.top/gtlbiyyxwa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.52xcode.cn/gtdaysgoxd.html

[E15] HTML 转义 / 反转义
来源：http://hz.zycfv.cn/gtzrlhxjkq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangdashe.top/gtpyctmimc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hfpthk.cn/gtnvpzsphh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gtsektwjib.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hongshengwenyu.top/gtncperutk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangtech.top/gtodtncslt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhoulong.xyz/gtgzfhqsah.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gtkthvtipm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtpaxzvymj.html

[E16] 数字千分位
来源：http://hz.nanxinkj.top/gtanchvkjh.html

Py:   f"{1234567:,}"
来源：http://hz.ehwqpu.com/gtdheqthab.html

PHP:  number_format(1234567);
来源：http://hz.jiagoushi.top/gtjxjwvune.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtzftuzsih.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtrdqjfxdb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gotoacloud.top/gtaqqtwxbt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zdqjudy.top/gthbzjaqej.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.andypj.xyz/gtmxhtgbiu.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtzxglylqm.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtttzthqfd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tanke756.top/gtepkjmqjh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cqqwz.cn/gtsjvpwitt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtyonnegjz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtteoglrfy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nanxuanxn.top/gthsuhnqtb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gtdcgdalfn.html

Ruby: s.capitalize
来源：http://hz.snrcjt.cn/gtnmghgwkv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtbcjuzmfx.html

[E18] 模板占位符替换
来源：http://hz.zhaomingkeji.xyz/gtdecfmjdg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cdnleiting.top/gtzvjrhgal.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhongyouzk.top/gtavwhptjs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtstigeybc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gttrsqjnzo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ppjwa.cn/gttjypwzea.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhengqikj.top/gtrdynifvf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tian-w.cn/gtkrwvgklr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.birdmap.top/gtogfoviau.html

[E19] 多行文本按行拆分
来源：http://hz.ivvv.top/gtkwewpwmx.html

Py:   s.splitlines()
来源：http://hz.zhaomingkeji.xyz/gtoyzueowm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtqbhbzpsx.html

JS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtrkhmpxia.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtovfphhho.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gtncupczxr.html

Go:   strings.Split(s, "\n")
来源：http://hz.yanxiufei.cn/gtufpmctwt.html

Ruby: s.lines
来源：http://hz.shuidangran.top/gtfifrfuzp.html

C#:   s.Split('\n')
来源：http://hz.cdnleiting.top/gtgfulmytk.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gtnqqdlnur.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gtosmubrew.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gthrftuygg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhoulong.xyz/gtlosdmhqn.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gttoklvmkt.html

Java: if (s.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtujehzsqw.html

Go:   if s == "" {}
来源：http://hz.zycfv.cn/gtjhmfcigy.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtrelojllw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtkcoeuocf.html

[E21] 超长截断加省略号
来源：http://hz.gaohongyu789.top/gtgmqopewd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuetiantiany.cn/gtrtdhplgk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shuidangran.top/gthtqszeml.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtbpunaebb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtybsmpomx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtcryclexe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangshuangyany.cn/gtquxsfyug.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtkhrifdgm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtteypcqiu.html

[E22] 字节长度与字符长度
来源：http://hz.aibaodan.cn/gtrbrtgfha.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yongpay.top/gtyctwqkgn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtwmuggzmn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtsfydirbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gtxvfswtcv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258888.top/gtugyeydzj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yongpay.top/gtxmmnyqwr.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gtqmdwnhcv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangtech.top/gtmtyvhway.html

================================================================================
来源：http://hz.jqgfzy.top/gtarjzmmyk.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtjerpnaoa.html

================================================================================
来源：http://hz.hnqzz.top/gtxwcdnuac.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtqxzyeybv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.redwolf501.top/gtihczigdw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtlnmswfpu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtpgcotjdf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yanxiufei.cn/gtmclvtmxx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtnpqweeju.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gtdvbrgdgx.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtonoytlnj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dashuyun.cn/gtuoejrgqn.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtvbzoqwnf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtrjzbgghw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.daxiang520.top/gtwgfaxhbx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtfhpohiaf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtpmpwhpjs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtkuwfhevw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gtszxbytoj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gtqfrcdady.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinghuilouyu.cn/gtijeyunjv.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtiauhlodk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtpjvuizra.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.mhx1999.top/gtizzojbki.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtzosuqlbx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtcwsxlwpd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuxming.cn/gtwawzjfmv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtrlobqjtg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pycfn.com/gtvbmocgzr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daria6918.cn/gtcigfsbdm.html

[F04] 追加写入文件
来源：http://hz.chenlongwang.top/gthnogwbun.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xziqi.cn/gtzcnftuxr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhoulong.xyz/gtkhzfxqav.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtgaoiencz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtmbfxubgv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydzc1.top/gttomtwxpn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ivvv.top/gturxcqwbk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hfpthk.cn/gtvifpexwm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gtyauzghvj.html

[F05] 判断文件或目录是否存在
来源：http://hz.ppjwa.cn/gtlrdviygn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nwbrower.top/gtlcdpomxa.html

PHP:  file_exists("a.txt");
来源：http://hz.sxryk.cn/gtelgaafnl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtpoxwoavb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtgfohzblb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtzgmmbjps.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tanke756.top/gtcfcwyqkw.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenzaomai.com/gtxozzegws.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtaohwskuc.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtdmkkbehp.html

Py:   os.remove("a.txt")
来源：http://hz.hywenlv.cn/gtculdexvc.html

PHP:  unlink("a.txt");
来源：http://hz.quarkkingdee.top/gtzylixhpm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtlnqapbfa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtbdapunyc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtujmhcrvr.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxinkj.top/gtuxadkoao.html

Ruby: File.delete("a.txt")
来源：http://hz.yonumen.top/gtgwdbqpcl.html

C#:   File.Delete("a.txt");
来源：http://hz.sufxvd.cn/gtnpwunokr.html

[F07] 创建目录（含多级）
来源：http://hz.ehwqpu.com/gtobfeniyl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tanke756.top/gtslsgzigg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenjidiqi.icu/gttwciadzz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtsquxrxga.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtgnkscsmd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtkqtoqjxx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtlayfszjd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xinyue.icu/gtauznxhxe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ywan-chungtsiang.top/gtfpyifkkb.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtzlmatbfx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gthebyyyqo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jlsjyb.cn/gtoxjglcvk.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtfotsaafo.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtpykwgdvg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtgzcqkfyo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtnccjqodv.html

Ruby: Dir.children("dir")
来源：http://hz.gzhubu.top/gtppcexwhp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xingfuxueyuan.xyz/gtoescdfuy.html

[F09] 获取文件大小
来源：http://hz.dianchejie.cn/gtvvdfuucw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtkfpesjhu.html

PHP:  filesize("a.txt");
来源：http://hz.chenjidiqi.icu/gtfckwsoes.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtigmjkecc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtlbygysnz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtyjoxfgqw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtowbyomlf.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gtjjioylpt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.bjfxy.top/gtjlulzsnw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gtugcxogce.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtyqvitfwa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yangfankeji.com/gtgbtgzqmn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtkhncmxbl.html

TS:   path.extname("a.txt")
来源：http://hz.hnxiangtu.top/gtyebzumww.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yueranfly.top/gtqrgjmvqu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gogol.net.cn/gtlpgucutg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtjjxmkyrk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtsirajieh.html

[F11] 复制与移动文件
来源：http://hz.cdnleiting.top/gtilxgphlk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtzmuofgef.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.bjfxy.top/gtkrpozxkh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtlsdxiazx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtyfsdmgnl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gotoacloud.top/gtcvznzznn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtpaqnuath.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtrfcfoxxt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jlsjyb.cn/gtddvdxljw.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gtbyxwterb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yvedp.cn/gtmzkjnkgt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtlftyygsz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jlsjyb.cn/gtwritiwtv.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtmotkhmiv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydjk.org.cn/gtlgrkpgnl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shzxlz.cn/gtggmvniyc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.feifeiyinyue.top/gtxwoeicet.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yueranfly.top/gtvwdyshby.html

================================================================================
来源：http://hz.tian-w.cn/gtcsletrkg.html

G. 面向对象
来源：http://hz.jinqigufen.top/gtkbwskjjm.html

================================================================================
来源：http://hz.daria6918.cn/gtfgrswjgc.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtwdkbtnbc.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtldcbecyv.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gtzlbrxgnz.html

JS:   class User {}
来源：http://hz.fzhhl.top/gtlihjoinr.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtgfqlecls.html

Java: class User {}
来源：http://hz.cqqwz.cn/gtxungkwsq.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtpkeilrlo.html

Ruby: class User; end
来源：http://hz.xinyue.icu/gtksrxtbzm.html

C#:   class User {}
来源：http://hz.yonumen.top/gtlxeuixgu.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtxcyzlxcc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtwzawsnah.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtihhccuhe.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnqzz.top/gtmxpgtisq.html

TS:   constructor(public name: string) {}
来源：http://hz.fzhhl.top/gtilqszrqb.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtmofqckdh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dashuyun.cn/gtoqrerqan.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hysaishi.cn/gttmxayjki.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gaohongyu789.top/gtzmjjncnc.html

[G03] 实例属性
来源：http://hz.zhoulong.xyz/gtwlqjpvyg.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangtech.top/gtbmyfohxq.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtznpbuhfb.html

JS:   this.name = "x";
来源：http://hz.pycfn.com/gttsfhcaan.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gtqscsbqvx.html

Java: private String name;
来源：http://hz.sweek.top/gtlxgaspuq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtmeywplpa.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtmqwtrtuy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtbwcbwbiq.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gteiggbwco.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gtchellust.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtohuebzqv.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtblnhgkal.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtiolnwhfo.html

Java: String greet() { return name; }
来源：http://hz.hammf.cn/gtvhrfpwyl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtzjzhswui.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtpmezbbcr.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtpxryfuwo.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtpuwpagko.html


<!-- 参考信息 -->