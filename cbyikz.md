代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gtwjntacuv.html

TS:   s.split(",")
来源：http://hz.shzxlz.cn/gtajdcgqum.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuetiantiany.cn/gtsckqgzbg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydzc1.top/gttmetrbhl.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtiflpewlx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xuetiantiany.cn/gthknvmvzk.html

[E08] 数组按分隔符合并
来源：http://hz.jiagoushi.top/gtzjwhkjdy.html

Py:   ",".join(items)
来源：http://hz.ivvv.top/gttnqmapwk.html

PHP:  implode(",", $items);
来源：http://hz.aibaodan.cn/gtkzvoksgf.html

JS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtnagekayr.html

TS:   items.join(",")
来源：http://hz.gotoacloud.top/gtywilgbkl.html

Java: String.join(",", items)
来源：http://hz.jinqigufen.top/gtwjhvmqyf.html

Go:   strings.Join(items, ",")
来源：http://hz.gaohongyu789.top/gtpkcpjnyg.html

Ruby: items.join(",")
来源：http://hz.sweek.top/gtcvrlbark.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtkrmowksv.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtdnaomahi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gzhubu.top/gtddmblysx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yongpay.top/gtjsxsbeya.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtwmklwkfk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtcmdkwsfn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtvtpmokyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daria6918.cn/gtcnjzfmko.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtboupluyr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.redwolf501.top/gtcevqddep.html

[E10] 左侧补零 / 定长填充
来源：http://hz.meibo888.top/gtkymxchdo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtltrkhfuo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ydjk.org.cn/gtaajewiov.html

JS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtywvmzqke.html

TS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtkeulrjum.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtnpeatnnc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtqlkynvrf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hywenlv.cn/gttyijipxn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gttooolrte.html

[E11] 反转字符串
来源：http://hz.iojbl.cn/gtmdykkzcc.html

Py:   s[::-1]
来源：http://hz.hysaishi.cn/gtuuvvliin.html

PHP:  strrev($s);
来源：http://hz.ybcxt.top/gtwwcsorye.html

JS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtssgnnaid.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtowkeysng.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tanke756.top/gtneiagsla.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.quarkkingdee.top/gtppkiqabs.html

Ruby: s.reverse
来源：http://hz.jlsjyb.cn/gthmaayqry.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtfzareuvw.html

[E12] 统计某字符出现次数
来源：http://hz.ehwqpu.com/gtcptqdmkf.html

Py:   s.count("a")
来源：http://hz.iojbl.cn/gtnyxqymmc.html

PHP:  substr_count($s, "a");
来源：http://hz.hammf.cn/gtuhwyhxls.html

JS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtmbjfvvcn.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtkwzmykvr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gtjmhdzpjw.html

Go:   strings.Count(s, "a")
来源：http://hz.snrcjt.cn/gtzdhfzqmh.html

Ruby: s.count("a")
来源：http://hz.dashuyun.cn/gtyeoxzfec.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hfpthk.cn/gtimlcdxxw.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gtckbomuwn.html

Py:   for ch in s: print(ch)
来源：http://hz.daria6918.cn/gtuhoqqcrm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.0kj1m.cn/gtveaovmpq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtxzhuosmb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtrdjvlfjd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shangyingyoupin.top/gtyzrrrpqt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.iojbl.cn/gtwhmevehp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtzggtxogm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gaohongyu789.top/gtefcmpnbr.html

[E14] URL 编码与 Base64
来源：http://hz.ywan-chungtsiang.top/gtterikcho.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtwvdztwhy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sufxvd.cn/gtcbywxsbm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gtoscrxesd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yueranfly.top/gtugyxoxyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenzaomai.com/gtanqlbnmc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtlkbejyqk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtjbijgwdk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hywenlv.cn/gtajadxxmy.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtocszeuyo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhengqikj.top/gtvuyrmove.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.snrcjt.cn/gtbgiglild.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gtbifojlzq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.andypj.xyz/gtxqqrowzv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtvmtvxlrt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gaohongyu789.top/gteetemcix.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gaohongyu789.top/gtmjbhamww.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jianghu66.top/gtafvwbvba.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gttigdqxvj.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtppwcbdrp.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtddudzahz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtmcygkejt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtmoberciv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtvwpjdesk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtzqaoniiq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydjk.org.cn/gtyrzfztje.html

C#:   1234567.ToString("N0")
来源：http://hz.zhoulong.xyz/gtstlsbhuu.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gteoipcaxw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgufenzy.top/gtsmkfgkfs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtfprfofrr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtxhxbxzts.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtmtldywuv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gthkhtivgn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtnxuiarsj.html

Ruby: s.capitalize
来源：http://hz.ydjk.org.cn/gthpckspgj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtuqltgasu.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtclmtajcj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzhubu.top/gtqnltttlb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtumoidxal.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtnmuuqtog.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gthiwvdxdc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cheryme.top/gttozndbxu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pengpengdd.cyou/gtozknedxd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gogol.net.cn/gtdilwanmc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtqyqpljeo.html

[E19] 多行文本按行拆分
来源：http://hz.tanke756.top/gtzuewxhgm.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gtkojzygoq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtwtslgewe.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtknmlvhlv.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtmzntbmcz.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtsooeaiql.html

Go:   strings.Split(s, "\n")
来源：http://hz.zdqjudy.top/gtagvfowud.html

Ruby: s.lines
来源：http://hz.yonumen.top/gtnknlhrye.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtsqmjwxda.html

[E20] 判断字符串是否为空
来源：http://hz.jianghu66.top/gtbtzzplto.html

Py:   if not s:
来源：http://hz.pengpengdd.cyou/gtqttmihbz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydzc1.top/gtuoednrgw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.316326.xyz/gtrlxmfbxy.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gthjtpnzhg.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigufen.top/gtfgqfnxul.html

Go:   if s == "" {}
来源：http://hz.zhongyouzk.top/gtqvzybsmh.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtntcrlgnp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtdrnpcase.html

[E21] 超长截断加省略号
来源：http://hz.zhongyouzk.top/gtxfeoykvp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yongpay.top/gtfmjvghvu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.iojbl.cn/gtexqtfjsi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtndisyous.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtzckrkxvw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtmxurlcmn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shuidangran.top/gtobzaafyt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.meibo888.top/gtvhjawrhc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtssvjgusc.html

[E22] 字节长度与字符长度
来源：http://hz.gotoacloud.top/gtaqfqspbx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtujegaqgr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtypskcciy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtygnryvsr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gtbgzkbyhe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hammf.cn/gtkdormxnt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hfpthk.cn/gtebhhodsh.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtdtggsdkp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtqxjpmyoh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjsfkybjd.html

F. 文件与目录
来源：http://hz.yj20258.top/gtqpxztlrw.html

================================================================================
来源：http://hz.cdnleiting.top/gteqfgpnws.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtulvjnyzk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.meibo888.top/gtdeyozmoa.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtgvjpoorz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtuasoyrdf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenzaomai.com/gttullriqs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtnnfqqnop.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hysaishi.cn/gtfmhqkltz.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtpnvresur.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pycfn.com/gtdnuhhcss.html

[F02] 逐行读取文件
来源：http://hz.quarkkingdee.top/gtdsztveiq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gtpetrikmr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtionrgwpz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtysegcnxs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtvwphgmuj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtmvnccezv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtcltdgzkq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.quarkkingdee.top/gtvuahdeql.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtheirfrtl.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtpuabguph.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtwamwlupy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtwbiobaho.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtxnybwszs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtphsoueon.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gaohongyu789.top/gtfvfusdcu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtzlccygak.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.iojbl.cn/gtxekwddkj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtquxcuyne.html

[F04] 追加写入文件
来源：http://hz.pycfn.com/gtmxvwucnz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtpuvkyufy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtlfgoakxz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtmaktbcuu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtpkocwopc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydjk.org.cn/gtyycwagqx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtvuytqcws.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtxhagvlov.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtccewjsfa.html

[F05] 判断文件或目录是否存在
来源：http://hz.yonumen.top/gtjallhvyb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhiwuduotai.top/gtpiejxioh.html

PHP:  file_exists("a.txt");
来源：http://hz.feifeiyinyue.top/gtxkskjbhp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtnqvmyiqa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtdxtqzask.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtgmzoylvb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtprqxqhop.html

Ruby: File.exist?("a.txt")
来源：http://hz.zycfv.cn/gtwrkmtjcw.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgfzy.top/gtbkmmajuc.html

[F06] 删除文件
来源：http://hz.iojbl.cn/gtdzezqrzr.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtoxhcarmx.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gttcgawhoa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtewaxzesi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtoosmphkz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtpfbcupkf.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtctavtssw.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxuanxn.top/gtgibzhfkb.html

C#:   File.Delete("a.txt");
来源：http://hz.jinghuilouyu.cn/gtenunicoq.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtniswynmp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hfpthk.cn/gtvhzdiwvv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtncfrpejj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtkthwsljx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtpgnhxctd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenlongwang.top/gtthmltmyv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cqqwz.cn/gtrmhvlsqw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtikwnkfkt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtkaitqicx.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gttvzwjoeq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtwnvjxhar.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cucudq.cn/gtqcwyqmtj.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtyvwyyssx.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtxkpksdtv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtrvqwrzmf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtmccljbyk.html

Ruby: Dir.children("dir")
来源：http://hz.nwbrower.top/gttaeprdiw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuanzx.com/gtashefntg.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtembybzep.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gtnyocgjzj.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtvbhtuksn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtopzcxntr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtqilhqfkn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtucrtkhvb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yongpay.top/gttvtvhktb.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gterizwlji.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtkdjoveyk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtqaoxdcki.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtmbnbrhvn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gtawjhchra.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtvfwsrvqu.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtkavulpmm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cucudq.cn/gtypnbmqyg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtobzalvfx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtlgtaagpn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtsjzpucnw.html

[F11] 复制与移动文件
来源：http://hz.daxiang520.top/gtdpxbxxye.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtwdohyifa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinghuilouyu.cn/gtuxowpauc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtfyurgtqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtqduzxckk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhongyouzk.top/gtqvkntvrg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtydoiohcr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gturcbdiir.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxinkj.top/gtdabbmcsb.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gtxpxsggzl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.kuanghao11.cn/gtdddtuzde.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhixingplan.top/gtqimbeqlw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gtjelyxowj.html

TS:   // 同上
来源：http://hz.jinqigufen.top/gtfoklizel.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jiagoushi.top/gtoibffjdr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtdihcgrdh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sweek.top/gtzipvsfhf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gtsxslkhtg.html

================================================================================
来源：http://hz.9152youxi.cn/gtpalpyijj.html

G. 面向对象
来源：http://hz.aizwys.cn/gtqszteyla.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvhbrppzk.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtyyxenzeb.html

Py:   class User: pass
来源：http://hz.cheryme.top/gtfsrktpqz.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gtlgxjkhgl.html

JS:   class User {}
来源：http://hz.yongpay.top/gtkcjzvatv.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gthjeqyynx.html

Java: class User {}
来源：http://hz.yueranfly.top/gthslfwhjb.html

Go:   type User struct { Name string }
来源：http://hz.xziqi.cn/gtdmjfangi.html

Ruby: class User; end
来源：http://hz.svipenyu.cn/gtczspxafa.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gteojzwzbc.html

[G02] 构造函数
来源：http://hz.yj202588.top/gtbjtqzyge.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtjjzfttzi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.feifeiyinyue.top/gtmolzdwtf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtzlnbgqpg.html

TS:   constructor(public name: string) {}
来源：http://hz.shuidangran.top/gtdlwqifsn.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtjqelfstp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtmyhrjasb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtsmahisqa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenzaomai.com/gtzpdbitoj.html

[G03] 实例属性
来源：http://hz.zhengqikj.top/gtlmqtidos.html

Py:   self.name = "x"
来源：http://hz.gotoacloud.top/gtpwlitqgn.html

PHP:  public string $name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtefjkfphh.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtwmymdqxs.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gtaoqphaya.html

Java: private String name;
来源：http://hz.52xcode.cn/gtrqunzbee.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtivlkjgaj.html

Ruby: @name = "x"
来源：http://hz.gotoacloud.top/gtuwsnidpo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtajgpvwml.html

[G04] 定义方法
来源：http://hz.xziqi.cn/gtveyvvhqi.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtsmqolqxw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtcogquhnk.html

JS:   greet() { return this.name; }
来源：http://hz.mhx1999.top/gtqfqayapa.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gtikchrhlo.html

Java: String greet() { return name; }
来源：http://hz.zhoulong.xyz/gtbgaozgxo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtszgmyvpe.html

Ruby: def greet; @name; end
来源：http://hz.andypj.xyz/gtcgmtwncu.html

C#:   public string Greet() => Name;
来源：http://hz.hongshengwenyu.top/gtufkuukvm.html

[G05] 继承
来源：http://hz.ydzc1.top/gtolnabcyh.html

Py:   class Admin(User): pass
来源：http://hz.iojbl.cn/gtejyfapkj.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtdggdrtwp.html

JS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gthsftxwzh.html

TS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtqdehcrrn.html

Java: class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtlwckyije.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shuidangran.top/gtnzznojuh.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gtkbykyfjo.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtsmnabjul.html


<!-- 参考信息 -->