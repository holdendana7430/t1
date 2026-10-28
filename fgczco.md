代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtzsehzfwg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtnmoxwjxr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgfzy.top/gturgqruop.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.havefunace.top/gttsnxeobt.html

C#:   s.Replace("a", "b")
来源：http://hz.gzhubu.top/gtimvtyfhv.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtfmdmgfcn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.bjfxy.top/gtpmbbuibw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtjgroosep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fengsongda.top/gtwtuvtjjh.html

TS:   s.split(",")
来源：http://hz.smart0.xyz/gtqajoqfpi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ivvv.top/gttokzkbft.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gtflhqndvc.html

Ruby: s.split(",");  s.split
来源：http://hz.sweek.top/gtuznjvsrp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xinyue.icu/gtkcgbwfqk.html

[E08] 数组按分隔符合并
来源：http://hz.yuxming.cn/gtkxuevjdh.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtnchozyfl.html

PHP:  implode(",", $items);
来源：http://hz.xylfe.cn/gtxbberuni.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtpgwywyyy.html

TS:   items.join(",")
来源：http://hz.zycfv.cn/gtrxqkmmfu.html

Java: String.join(",", items)
来源：http://hz.sufxvd.cn/gtxdwforoi.html

Go:   strings.Join(items, ",")
来源：http://hz.yj202588.top/gtunmcgmgu.html

Ruby: items.join(",")
来源：http://hz.pengpengdd.cyou/gtfajrgchw.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gtsrsxibqk.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtkrhnyiyh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gthxcbyvjr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gtrhuyoerm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtkxymvyld.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtotmasecx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtlexkmouh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtafukolan.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxuanxn.top/gtadtheqia.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangtech.top/gtvebrfunk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258.top/gtopewqmgq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pycfn.com/gtnlxvzhxy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dashuyun.cn/gtlxxfgnbu.html

JS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtgxdvazbh.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtgkgdlmhu.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtfznxujbk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nwbrower.top/gtchttrcze.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtyoapxvxl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xylfe.cn/gtnkqgzzjz.html

[E11] 反转字符串
来源：http://hz.andypj.xyz/gttruwyqri.html

Py:   s[::-1]
来源：http://hz.meibo888.top/gtfaakmlma.html

PHP:  strrev($s);
来源：http://hz.zhengqikj.top/gtsmoacvzf.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtydyubdai.html

TS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gteqajysbq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gttuoljcsl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.feifeiyinyue.top/gteqqvwhkz.html

Ruby: s.reverse
来源：http://hz.jinqigufen.top/gtexvfeayi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gttmmzrfub.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gtprzumjod.html

Py:   s.count("a")
来源：http://hz.meibo888.top/gtqnussoev.html

PHP:  substr_count($s, "a");
来源：http://hz.dashuyun.cn/gtmuhwxahu.html

JS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtpuxqtoso.html

TS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtaqttjwej.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtyfjwmgtr.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtempxdgbv.html

Ruby: s.count("a")
来源：http://hz.quarkkingdee.top/gtdsqwnopo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shzxlz.cn/gtiyxvfsso.html

[E13] 逐字符遍历
来源：http://hz.birdmap.top/gtdgqbckqk.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtulxjhlbo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.haohaochexian.top/gtozuhrsne.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gttufsigya.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gttrexgfbh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hongshengwenyu.top/gtkmnldwpl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinyuanbaomall.cn/gtudafytbb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.mhx1999.top/gtksqfshql.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.chenjidiqi.icu/gtbgsfkqak.html

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtbtycufmc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.316326.xyz/gtszplouum.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gttkychoft.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pengpengdd.cyou/gtfwpgduvh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.haohaochexian.top/gtjudkbzcq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cashguo.top/gtogxjwxfd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gotoacloud.top/gtxaxpmmie.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtmihadoqs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cdnleiting.top/gtiwkdganv.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigufen.top/gtrdksarno.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ywan-chungtsiang.top/gtvsnbhqvr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtdelvtohk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hongshengwenyu.top/gtezeoujtr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangkeji.top/gtynkfsdnr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xylfe.cn/gtozsufums.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenjidiqi.icu/gtkfushsho.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtieaywlvp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuanzx.com/gtgskhuphl.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtoxvvffev.html

Py:   f"{1234567:,}"
来源：http://hz.pengpengdd.cyou/gthrfkwaoz.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangtech.top/gtoykexpfp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtijdvjvwb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gtkbucbyvy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hfpthk.cn/gtzgvtojmd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenjidiqi.icu/gtwnzcnaxp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhaomingkeji.xyz/gtcmmdbcfg.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtbrqlekmk.html

[E17] 首字母大写
来源：http://hz.hywenlv.cn/gturahwbze.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtydgwlink.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgfzy.top/gtqfcfabjh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtiamcscrf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtkrhfpjwr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtczcplrnv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtiwhnybbj.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gtjzblmads.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gtqyknypka.html

[E18] 模板占位符替换
来源：http://hz.jinghuilouyu.cn/gtjiyaqsxh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yongpay.top/gtghmomrmy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gtfosjcvpd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtienbgskr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtnvnnretu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtndnvpfsc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jlsjyb.cn/gtsboauhvt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtarygqhdb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtlnbutemy.html

[E19] 多行文本按行拆分
来源：http://hz.c1oappe.top/gtmhhzmpyn.html

Py:   s.splitlines()
来源：http://hz.hysaishi.cn/gtfnwkypos.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtxwoiwshk.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtfaqswgbl.html

TS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtsxertgnu.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtrcivfodz.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtegczzhaj.html

Ruby: s.lines
来源：http://hz.yangfankeji.com/gtlvyhtzji.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtfdtrgkrz.html

[E20] 判断字符串是否为空
来源：http://hz.dianchejie.cn/gtsarbynfm.html

Py:   if not s:
来源：http://hz.wangdashe.top/gtghjdetue.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtyctlaexe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gzhubu.top/gtjkuaqohh.html

TS:   if (s === "") {}
来源：http://hz.smart0.xyz/gtievwpleo.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gtgctgqmcl.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtkyflamhe.html

Ruby: if s.empty?
来源：http://hz.jianghu66.top/gtqpywahiv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtlasrvfeg.html

[E21] 超长截断加省略号
来源：http://hz.nwbrower.top/gtdamtngym.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258888.top/gtxulijtnl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtjglsikpc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtdanrmdhs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtahmffhsf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtawovgtbo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.snrcjt.cn/gtupgqlrmc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cqqwz.cn/gtrfxwlqgd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gtgtxdsxnc.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtfvqsdhih.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gtamnzzcwi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtkiryezxz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtsgsslpnp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtaqqftgrl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xinyue.icu/gtevzanhjb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gogol.net.cn/gtxanwxfnm.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangshuangyany.cn/gtewwmcmrr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gtldirwtxl.html

================================================================================
来源：http://hz.xylfe.cn/gtiismnpya.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtpcbeaywb.html

================================================================================
来源：http://hz.zycfv.cn/gtubxtxvuh.html

[F01] 读取整个文件
来源：http://hz.meibo888.top/gtcxdnhpvn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtbcevmhfz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daxiang520.top/gtbfwlpdmw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gttuifhtak.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj202588.top/gtevgurcbs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gthkkhhdlr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtwdinyqoj.html

Ruby: File.read("a.txt")
来源：http://hz.zycfv.cn/gthhctxeqq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtxfjzsugo.html

[F02] 逐行读取文件
来源：http://hz.iojbl.cn/gtsxqivtsa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jianghu66.top/gtzqslrfnu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.daxiang520.top/gtgrvhvnzc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtzalvwdil.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtxooilthd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gttqtaujxy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigfzy.top/gtmmaszaqv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhiwuduotai.top/gtaoiakznw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yongpay.top/gtbcyzfrzb.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtbmxzhigk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guowangkeji.top/gtunzjqwam.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtkzwmtcfj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtuvsxukyy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtwbgljzix.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtbigiylse.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydzc1.top/gtoyznlbqj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pycfn.com/gtrajbptsq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gtojbmkzmn.html

[F04] 追加写入文件
来源：http://hz.xylfe.cn/gtetgypnwr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gtmrvogfjo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtqgmbzawq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtaxsnxwza.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtgixqzoac.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangshuangyany.cn/gtbamhbmfv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtcynzzslw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fengsongda.top/gtimfjuxvq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.52xcode.cn/gttxrojaxj.html

[F05] 判断文件或目录是否存在
来源：http://hz.mhx1999.top/gtsaqzipgf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhiwuduotai.top/gtzhqybici.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtqlpexhzs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtkwycvrpq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtszamctub.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtywucclnh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhaomingkeji.xyz/gtdytryvqn.html

Ruby: File.exist?("a.txt")
来源：http://hz.jyoumei.cn/gtneccevti.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtugtwbucf.html

[F06] 删除文件
来源：http://hz.yanxiufei.cn/gtwmmjinio.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gteycycyrh.html

PHP:  unlink("a.txt");
来源：http://hz.mhx1999.top/gtfmvvnqic.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtkursqypw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtvflgsybk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtethreozg.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gtwxkcpnfo.html

Ruby: File.delete("a.txt")
来源：http://hz.sweek.top/gtfbxlqsre.html

C#:   File.Delete("a.txt");
来源：http://hz.xuetiantiany.cn/gthibcopgb.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtchqgtfkz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydzc1.top/gtxaakdkdy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtdsdrdmxw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtfxvknjgm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtrdrplvjk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtytoxjnhy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shzxlz.cn/gtsztqesjt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhaomingkeji.xyz/gtfdwycanu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtfzlefckp.html

[F08] 遍历目录
来源：http://hz.zhoulong.xyz/gtfyrbstig.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yonumen.top/gtbagmhzrr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhijiandao.cn/gtypggtvpg.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtlntcnmiq.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtyzszbqcd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtzllqbyhh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gtlkmueplv.html

Ruby: Dir.children("dir")
来源：http://hz.jiagoushi.top/gtmzcwknpw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gotoacloud.top/gtjcxfhbqv.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtqlknwkds.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenlongwang.top/gtdwaqxnrk.html

PHP:  filesize("a.txt");
来源：http://hz.zhengqikj.top/gtslckkecl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtmwwwemhj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gthzduykyi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtbvnaodzf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnxiangtu.top/gtpszpcxts.html

Ruby: File.size("a.txt")
来源：http://hz.hongshengwenyu.top/gtxgusgycb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtqgvuiido.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtioyxwugk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtyqdysmnq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xinyue.icu/gtlrevnqqn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtolnkuvfu.html

TS:   path.extname("a.txt")
来源：http://hz.ydjk.org.cn/gtiqjsgxcg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guannengcc.top/gtjtaixhwh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ppjwa.cn/gthzjndmug.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtozzqepai.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gtyhwokcvk.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtmckjohci.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtdjulzgtx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pengpengdd.cyou/gtdfbnddam.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtbekqefjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtcybjainx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtcukuufyu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.birdmap.top/gtpatmkmfv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtkmitcoal.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jianghu66.top/gtdnhqnpte.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtatrfnjzs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtahgugkar.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gtiqdptkva.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jlsjyb.cn/gtromrwfms.html

TS:   // 同上
来源：http://hz.316326.xyz/gtdvfwfpit.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtalbjmbtq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtyhfrgtkf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtdtmgqcpd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtojgltbgt.html

================================================================================
来源：http://hz.yuanzhike.top/gtodkdaxny.html

G. 面向对象
来源：http://hz.sxryk.cn/gthzyovojs.html

================================================================================
来源：http://hz.xuanzx.com/gtlxcqlnhk.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtxphdegfj.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gtysdcdjja.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtazjlujkl.html

JS:   class User {}
来源：http://hz.andypj.xyz/gtmwlknixe.html

TS:   class User { name: string = ""; }
来源：http://hz.chenlongwang.top/gteqlmlxvi.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtnwlqgvlt.html

Go:   type User struct { Name string }
来源：http://hz.hywenlv.cn/gtswlfvztj.html

Ruby: class User; end
来源：http://hz.daria6918.cn/gtsfqrzphn.html

C#:   class User {}
来源：http://hz.bjfxy.top/gtyztmomel.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtqwmimgvk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gteneyfvmf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtmcrsbhqm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cheryme.top/gtjujakuye.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtuekxqtup.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtlzjuxajy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cucudq.cn/gtroknpmib.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtzllrpumh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ybcxt.top/gtdbsaidld.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gtcoamcapb.html

Py:   self.name = "x"
来源：http://hz.ydzc1.top/gthfhagqdf.html

PHP:  public string $name = "x";
来源：http://hz.zhijiandao.cn/gtzacmonyq.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtisryfxls.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtvjznsavc.html

Java: private String name;
来源：http://hz.sysykeji.top/gtdyuowkid.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.mhx1999.top/gtfyiwglar.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtkizqalcd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.quarkkingdee.top/gtplllekko.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gtbvnegfuv.html

Py:   def greet(self): return self.name
来源：http://hz.hammf.cn/gttisiaegf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtmxzwubtc.html

JS:   greet() { return this.name; }
来源：http://hz.yvedp.cn/gtyavyxztl.html

TS:   greet(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtufnhqfiy.html

Java: String greet() { return name; }
来源：http://hz.fzhhl.top/gtajosvfby.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtzlzodfjf.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtyisqseel.html

C#:   public string Greet() => Name;
来源：http://hz.hysaishi.cn/gtemxgdfmw.html

[G05] 继承
来源：http://hz.cheryme.top/gtymyajivu.html


<!-- 参考信息 -->