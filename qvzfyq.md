代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gthyaramxa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtjkwrpvva.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hammf.cn/gtjjjrurdd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.smart0.xyz/gtjvidglag.html

C#:   s.Replace("a", "b")
来源：http://hz.gaohongyu789.top/gttjoiyqwh.html

[E07] 按分隔符拆分
来源：http://hz.xingfuxueyuan.xyz/gtxnlaelqo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuxming.cn/gtlpibtfqd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ivvv.top/gtkwaqrebu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zycfv.cn/gtfaxmrjfh.html

TS:   s.split(",")
来源：http://hz.tanke756.top/gtrxuzeude.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.birdmap.top/gtidofaqfs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gtnaexjjyk.html

Ruby: s.split(",");  s.split
来源：http://hz.yongpay.top/gtghcgpiux.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.iojbl.cn/gtwsjsfetl.html

[E08] 数组按分隔符合并
来源：http://hz.hnqzz.top/gtbaibvjru.html

Py:   ",".join(items)
来源：http://hz.jiagoushi.top/gtbptaqaoh.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gtyowtxdqf.html

JS:   items.join(",")
来源：http://hz.yvedp.cn/gtshkllnzc.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtanulpnsf.html

Java: String.join(",", items)
来源：http://hz.vqdsnc.cn/gtpjhsacbz.html

Go:   strings.Join(items, ",")
来源：http://hz.mhx1999.top/gtcdqvflty.html

Ruby: items.join(",")
来源：http://hz.cqqwz.cn/gthxoyazmu.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gtwwkaojjr.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtlzkcovkr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258.top/gtdnziduyk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jianghu66.top/gtebpgguqf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtdboumozy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtugzseane.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtrdzvlfia.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hongshengwenyu.top/gtqkichjcp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhijiandao.cn/gtkknsgbfe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yanxiufei.cn/gtetaxqzzi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.wangdashe.top/gtkrapmxtt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtlezejkil.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxinkj.top/gtvwrenciy.html

JS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtdhcixwcn.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtzeapzrab.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigufen.top/gtrocrhceu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nwbrower.top/gthszkxjxa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtaduktser.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtfahtrgou.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gthdbwgfol.html

Py:   s[::-1]
来源：http://hz.cashguo.top/gtskgzswbh.html

PHP:  strrev($s);
来源：http://hz.guannengcc.top/gtlutcdojd.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gthuyvigsz.html

TS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gthbxkbpdv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.iojbl.cn/gtsdrcinud.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.svipenyu.cn/gtcwhrpcvo.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtrrnposdu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtdbumnehp.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtwjrgjzdr.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtvdtzoowc.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxuanxn.top/gthrjjnjmy.html

JS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtjqipakzx.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtktgnzdwm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtgxnvifrf.html

Go:   strings.Count(s, "a")
来源：http://hz.chenjidiqi.icu/gtbachalrl.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtqljpthpu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yueranfly.top/gtvthjllpd.html

[E13] 逐字符遍历
来源：http://hz.wangdashe.top/gtoaskrcdt.html

Py:   for ch in s: print(ch)
来源：http://hz.sxryk.cn/gtpvffupmz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangtech.top/gtuavxlazs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtsdjntwjn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtfbctxcnx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtjbcaroni.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtlzbxsxno.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.havefunace.top/gtjgcrzzos.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gtbojkdfku.html

[E14] URL 编码与 Base64
来源：http://hz.sysykeji.top/gtevgqsgvl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.smart0.xyz/gtcgfmnyjv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhiwuduotai.top/gtsaridqdw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yonumen.top/gtlqrjdpwe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cheryme.top/gtkcgfgvqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guowangkeji.top/gtvjlkgunc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daria6918.cn/gtprkejpfx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gthqqcncpt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cqqwz.cn/gtkcsrcqhf.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtfjkxoiav.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtefriynmo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jianghu66.top/gtnhjvekop.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cqqwz.cn/gthbbmqczh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sweek.top/gtskjiaedc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtbyauxwsq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ywan-chungtsiang.top/gtkvhxipxx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pycfn.com/gtzlvzerxc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.birdmap.top/gtkgpvhcuz.html

[E16] 数字千分位
来源：http://hz.hysaishi.cn/gthpvcioni.html

Py:   f"{1234567:,}"
来源：http://hz.guowangkeji.top/gtprypptab.html

PHP:  number_format(1234567);
来源：http://hz.redwolf501.top/gtfxursfmo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gtuthyhfvy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtcwnfyhcq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ppjwa.cn/gtipifunek.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtzpvjqbbc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yanxiufei.cn/gtyjsgvvfs.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gtadnqiova.html

[E17] 首字母大写
来源：http://hz.zycfv.cn/gtrqnphhkw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtxovbsifm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shuidangran.top/gtgaywkwqs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtxxdrilmd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtaewutvwn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtxvtgmzcp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tian-w.cn/gtsyjzbzig.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtmrocurjd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nwbrower.top/gtwofjlvva.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gtpeeoxroc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sweek.top/gtjzvzvusa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.quarkkingdee.top/gtzpetnpki.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtyocnajkn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtgjwuyraj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtdrzwsjqc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shangyingyoupin.top/gtkfjsggfx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yongpay.top/gtaefqrcsk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtbmhpsyuw.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtczxlqevy.html

Py:   s.splitlines()
来源：http://hz.jyoumei.cn/gtgpoepywf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuanzx.com/gtlpfengfr.html

JS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtkobsjqkx.html

TS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtcwtqqjrd.html

Java: s.lines().toList()
来源：http://hz.meibo888.top/gtdfhdcidk.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhaomingkeji.xyz/gtlnhxxrwg.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtfnswfjvh.html

C#:   s.Split('\n')
来源：http://hz.jinyuanbaomall.cn/gtjftkvkva.html

[E20] 判断字符串是否为空
来源：http://hz.nanxuanxn.top/gtryklelkv.html

Py:   if not s:
来源：http://hz.gaohongyu789.top/gttshurjim.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtnvakbzjn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhijiandao.cn/gtkshpgibj.html

TS:   if (s === "") {}
来源：http://hz.yuanzhike.top/gtfobtjcmh.html

Java: if (s.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtjxcwaufo.html

Go:   if s == "" {}
来源：http://hz.yangfankeji.com/gtcetcaokm.html

Ruby: if s.empty?
来源：http://hz.zhiwuduotai.top/gtkhdzkoxx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yongpay.top/gtcvgyibbb.html

[E21] 超长截断加省略号
来源：http://hz.xingfuxueyuan.xyz/gtttumqoqf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtocdlimsv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xuanzx.com/gtobjpllmc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtlmuxzuth.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtyngeugun.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtqxvskfsr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhengqikj.top/gtatrliymy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtlmhydbav.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gtuuozffkf.html

[E22] 字节长度与字符长度
来源：http://hz.aizwys.cn/gtscqkkrre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtvchophgk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtnplkozqt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtxjsnzbsd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtvsmwlgmn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.316326.xyz/gtncauynrz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.snrcjt.cn/gtgywhsjrv.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangkeji.top/gtppsoeukc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtnvmmckze.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgzonelpy.html

F. 文件与目录
来源：http://hz.bjfxy.top/gtpbeavumt.html

================================================================================
来源：http://hz.yvedp.cn/gttjmkiyna.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtwdoshtzc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtsrbzttqe.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtwsdqtraj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cashguo.top/gtfnnytqns.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtktaeqqdw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtpkubzilv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cheryme.top/gtgfafprjh.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtutqyoewi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenjidiqi.icu/gtygfqobcd.html

[F02] 逐行读取文件
来源：http://hz.hnqzz.top/gtkrrgjwth.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnqzz.top/gtzrsziqvf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.kuanghao11.cn/gtmjqajavs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtautcijxq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtccmobosa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtoeojcpmz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydjk.org.cn/gttgsqxzlh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhengqikj.top/gtixklbfem.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ivvv.top/gtikarpvkg.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtwtzqsnso.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.quarkkingdee.top/gtgwvtjjgs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yongpay.top/gtnnpefpcd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtlmewpqyu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtmcpqqatx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.kuanghao11.cn/gteuwmwrff.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenlongwang.top/gtfdhypsfi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.svipenyu.cn/gtemxtapdc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtfltenkqc.html

[F04] 追加写入文件
来源：http://hz.shzxlz.cn/gtlntnmhhr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.316326.xyz/gtavgpzjnc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gtslagesix.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtebyrccyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtjlmqpnrw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtfnkogykv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.9152youxi.cn/gttlatvkoq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtmmzntdfq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhiwuduotai.top/gtrtwedobc.html

[F05] 判断文件或目录是否存在
来源：http://hz.cheryme.top/gtbgjzoitp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.kuanghao11.cn/gtymgymvcf.html

PHP:  file_exists("a.txt");
来源：http://hz.pycfn.com/gtqtitgpjl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtfpwlnpsc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtbuawgzhn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gthkccsnqk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtixluzjtc.html

Ruby: File.exist?("a.txt")
来源：http://hz.hongshengwenyu.top/gtnvswimyq.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtypykmihq.html

[F06] 删除文件
来源：http://hz.zhongyouzk.top/gtshvuxmal.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtkcyrphwd.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gtngwbgfwu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtguxvkhva.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtnimpfeib.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtchvztfsc.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtfmakrupf.html

Ruby: File.delete("a.txt")
来源：http://hz.tanke756.top/gtkerahvxs.html

C#:   File.Delete("a.txt");
来源：http://hz.yj202588.top/gtbvdjpusp.html

[F07] 创建目录（含多级）
来源：http://hz.shzxlz.cn/gtwfnoiewp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxinkj.top/gtzsjrsbtw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.aizwys.cn/gtzltgfmnp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtvctjkhhk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtmcqsscxy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.snrcjt.cn/gtckwlfyqu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuanzhike.top/gtcmbaxzxf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.52xcode.cn/gtngqwgpfs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtswlwlato.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtojcrrzjl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtxbxayznb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gtimkaomqe.html

JS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gteyztjagg.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtwooxwcoe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gthehhyjyo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydzc1.top/gtvxdilevs.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtbulrvwlu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuanzhike.top/gtygknyojn.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gthxbljkwg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtkbivozfh.html

PHP:  filesize("a.txt");
来源：http://hz.jinghuilouyu.cn/gtothpabkg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtzlnefwvb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtagysvbyo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtjtwmkmkz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gaohongyu789.top/gtjuctacxt.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtnmwbhtkz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtoaahvpyq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gtileczreq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtibnbtbbs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yvedp.cn/gtorjmilqr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gthbgzxazv.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtfvpzvhwc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ivvv.top/gtqhtypzpi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtelrtismz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtqdooccbq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gthffvxhkp.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtnlrttdzn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtxnpgferg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gotoacloud.top/gtjvljhzds.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtcdgdbitv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtndooapei.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtpsyhriyf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhongyouzk.top/gtcsupfymc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtzjnovqky.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dashuyun.cn/gtliwugdys.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtezyjgfhz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigufen.top/gtjyvuvbbg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtdkoytais.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtwtxourjm.html

TS:   // 同上
来源：http://hz.shanyushiyangtech.top/gtqpoiqrbo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtqrfafquk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtooryzipv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuanzx.com/gtptjaubsv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.daria6918.cn/gtmifgrpjh.html

================================================================================
来源：http://hz.chenzaomai.com/gtrxvskjjc.html

G. 面向对象
来源：http://hz.snrcjt.cn/gtaetkyput.html

================================================================================
来源：http://hz.yvedp.cn/gtomonofmr.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtvuxjmvid.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gttsgrsekv.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gttrmdnqxs.html

JS:   class User {}
来源：http://hz.svipenyu.cn/gtjtpusore.html

TS:   class User { name: string = ""; }
来源：http://hz.jyoumei.cn/gtcnxwgvey.html

Java: class User {}
来源：http://hz.jiagoushi.top/gtsyshlfso.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtcacbxary.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gttgyyzmse.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gtkdbitawt.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtekmgarwv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gotoacloud.top/gtwqovndej.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yanxiufei.cn/gtzcmclhnv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtrzihgmmz.html

TS:   constructor(public name: string) {}
来源：http://hz.sxryk.cn/gtvlwrktuy.html

Java: User(String name) { this.name = name; }
来源：http://hz.fengsongda.top/gtzbnxkxpj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tian-w.cn/gtwoxeibfi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtdawhdzcc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yvedp.cn/gtxysqmweh.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gtouicvaoi.html

Py:   self.name = "x"
来源：http://hz.pengpengdd.cyou/gtyyizrfoc.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtkhwaeczq.html

JS:   this.name = "x";
来源：http://hz.cheryme.top/gttngsxksz.html

TS:   name: string = "x";
来源：http://hz.ydzc1.top/gtxfuarroa.html

Java: private String name;
来源：http://hz.fzhhl.top/gtoxpkufiw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtyzqiurtr.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtfajgdess.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.haohaochexian.top/gtklfkpoue.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtakgqxcnr.html

Py:   def greet(self): return self.name
来源：http://hz.hysaishi.cn/gtipnlqlqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtqhixxvgk.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtqomntdka.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtsxlbuwdq.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtlexsogcf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sufxvd.cn/gtumbylwkc.html

Ruby: def greet; @name; end
来源：http://hz.fengsongda.top/gtzqzvsoex.html

C#:   public string Greet() => Name;
来源：http://hz.52xcode.cn/gtvkclvqfv.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtziqljhup.html


<!-- 参考信息 -->