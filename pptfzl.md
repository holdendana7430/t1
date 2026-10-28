代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhoulong.xyz/gtdlgiaskc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtcavexogs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.wangdashe.top/gtqxbtjvtb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtdagwyrlo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pycfn.com/gtiaefjpyg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhaomingkeji.xyz/gtaevuljod.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gthkxkgsar.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhongyouzk.top/gtcrjdvqpn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.daria6918.cn/gtcambizjt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sweek.top/gtwokxclzs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gtyehgmnjs.html

JS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtotblwyct.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtvqexbwwo.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtopwatcuq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tanke756.top/gtsbzgmvlo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.wangdashe.top/gtmmajclmj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gtticqdejs.html

[E11] 反转字符串
来源：http://hz.shanyushiyangtech.top/gtwxmdbedo.html

Py:   s[::-1]
来源：http://hz.gogol.net.cn/gtfykzyfsn.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtzqkkbleh.html

JS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtabhfsqfk.html

TS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtzydmjcsc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.52xcode.cn/gtswyplipd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtyowjddqh.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtjezxyijg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtpoisypxn.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtqioynyif.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtkwvhlgyg.html

PHP:  substr_count($s, "a");
来源：http://hz.wangdashe.top/gtnogsgbve.html

JS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gtqcdedcpc.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtifwlbwzg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zdqjudy.top/gtjxvqpxqx.html

Go:   strings.Count(s, "a")
来源：http://hz.316326.xyz/gtxqbfohgu.html

Ruby: s.count("a")
来源：http://hz.jqgufenzy.top/gtxuepfqns.html

C#:   s.Count(c => c == 'a')
来源：http://hz.haohaochexian.top/gtpgvavlzu.html

[E13] 逐字符遍历
来源：http://hz.yvedp.cn/gtczoqbyaw.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gthamtvrse.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gtcvwkwwwt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtzkrazyfz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gteplsuspr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yanxiufei.cn/gthdyotyss.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daria6918.cn/gtetkcygqp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.haohaochexian.top/gtasummkho.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtkqqcovma.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtdmngvueo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tianlin.xyz/gtacolivbf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtrsflmeqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhongyouzk.top/gtpduzqqjx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yonumen.top/gtszeioych.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gotoacloud.top/gtydhggypz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tian-w.cn/gtyeoixqwu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtccleckje.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtkxxqmhuz.html

[E15] HTML 转义 / 反转义
来源：http://hz.xingfuxueyuan.xyz/gtfioqkobq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ybcxt.top/gthsrgblrp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aizwys.cn/gtppdunfto.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yongpay.top/gtoeykgusq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yanxiufei.cn/gtzjubqomc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtpeeercoh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtwnruhtvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aizwys.cn/gttweuecxb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258.top/gtcxplkkys.html

[E16] 数字千分位
来源：http://hz.jyoumei.cn/gtroqlonct.html

Py:   f"{1234567:,}"
来源：http://hz.cucudq.cn/gtkpjmmhfe.html

PHP:  number_format(1234567);
来源：http://hz.tian-w.cn/gtqkxytywm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gthyqtbnnw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xziqi.cn/gtinefttyg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxinkj.top/gtcyzftpfu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydjk.org.cn/gtovxcwbag.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtkltngomc.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxuanxn.top/gtxpcdysfj.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtqfhkzdbg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hfpthk.cn/gtctvmonaa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gtzrexauxa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gttelyrvte.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gtnwxiuwsv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuxming.cn/gtcuyffdyv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gttxhixslc.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtglapmjcv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jyoumei.cn/gtsycopaal.html

[E18] 模板占位符替换
来源：http://hz.meibo888.top/gttccnlqlf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtpkbmogbi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtkaokzzjs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtrcvtjyzh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtsfqjjcfr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shzxlz.cn/gtvjnxamyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gtjzxsfjtz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ehwqpu.com/gtsxxspjog.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cheryme.top/gtqucxgvrl.html

[E19] 多行文本按行拆分
来源：http://hz.jinghuilouyu.cn/gtgoglmxut.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gtravcdmee.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cheryme.top/gtvbtkexuf.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtjsyvfyko.html

TS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gtqtgulqel.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gtqvsbblji.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtoosxqwnq.html

Ruby: s.lines
来源：http://hz.wangdashe.top/gtuefazpew.html

C#:   s.Split('\n')
来源：http://hz.xylfe.cn/gtcbuapgys.html

[E20] 判断字符串是否为空
来源：http://hz.tian-w.cn/gtyoftvxjv.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtsyagtpip.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhijiandao.cn/gtaailfoxv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhongyouzk.top/gtlcqzhfzp.html

TS:   if (s === "") {}
来源：http://hz.hongshengwenyu.top/gtikkrqddb.html

Java: if (s.isEmpty()) {}
来源：http://hz.guannengcc.top/gtgmnnaarm.html

Go:   if s == "" {}
来源：http://hz.pycfn.com/gtlsxytzup.html

Ruby: if s.empty?
来源：http://hz.yueranfly.top/gtnnobzeex.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtqflnucir.html

[E21] 超长截断加省略号
来源：http://hz.kuanghao11.cn/gtsvrcegpt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pycfn.com/gtdqrsgont.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aizwys.cn/gtszvkqlsy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtjwdltjad.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gthhociwnr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtrbsbuhpa.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtzillnsvu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nwbrower.top/gtxypimmtw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shuidangran.top/gtjwdadymn.html

[E22] 字节长度与字符长度
来源：http://hz.316326.xyz/gtiggxjmsh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtgtpswump.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtrbftemuw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtsvyjtmlo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtdxoellfw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.pengpengdd.cyou/gtgavvdcxc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ppjwa.cn/gtqnqmtxhn.html

Ruby: s.bytesize;  s.length
来源：http://hz.jianghu66.top/gtmarmiekh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.fengsongda.top/gthmawunak.html

================================================================================
来源：http://hz.aizwys.cn/gtbczsmsxq.html

F. 文件与目录
来源：http://hz.havefunace.top/gtbasdaqkh.html

================================================================================
来源：http://hz.316326.xyz/gttnorbeda.html

[F01] 读取整个文件
来源：http://hz.meibo888.top/gtaoxpuqrz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtquqbcczt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtqbnzkrcx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghu66.top/gtfsuxocgz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgufenzy.top/gtscoxskdf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtkaiasvyx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtdkdertbz.html

Ruby: File.read("a.txt")
来源：http://hz.sufxvd.cn/gtxkcfmisl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ivvv.top/gtwiylzqit.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gtjsggidok.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hammf.cn/gtmrcuvdcw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtwvrcfsto.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtxyzuphvh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtuwaouxaj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtbgpyiihp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuxming.cn/gtezozohdj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtzfnudhyt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jyoumei.cn/gturxcmerc.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtsjnjxkhr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.snrcjt.cn/gtbbnfmtvy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj202588.top/gtcrxfqweq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtmsgbuwrr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtaifslgtb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fzhhl.top/gtxsvfdmey.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtqysiblxz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tanke756.top/gtjkxjgzww.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtvcwzvfja.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtfqpzajtf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gtoseozaxj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhengqikj.top/gtncjrnmym.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtbvllikuf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtsegcvrtl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtlxqknlsx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gtyjwwdpqz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gtpjleqyoj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtxuqxwkqa.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydjk.org.cn/gtqscqcbfl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.c1oappe.top/gtzciapbth.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtarhgayeb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gttghnhtam.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtpaydeqgw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtzzttmdje.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgfzy.top/gthphtkxls.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gtcooohzny.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtxzjexwup.html

[F06] 删除文件
来源：http://hz.sweek.top/gtzhvvxceo.html

Py:   os.remove("a.txt")
来源：http://hz.cucudq.cn/gttoijpegv.html

PHP:  unlink("a.txt");
来源：http://hz.yj202588.top/gtdqzpzdso.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtmzzyjnxp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtdpwmgglx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtzwkjcmtr.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtlqrpjvzr.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gtmlnxalhz.html

C#:   File.Delete("a.txt");
来源：http://hz.gotoacloud.top/gtdwicaiun.html

[F07] 创建目录（含多级）
来源：http://hz.hnqzz.top/gttcfylmuy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtumoqaxhl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pengpengdd.cyou/gtscqqmzqd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtbiggqzic.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtylltxuxa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cashguo.top/gtuwfxsizc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.snrcjt.cn/gtvqbzjdqu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fzhhl.top/gtstorxzyk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sweek.top/gttgnszarj.html

[F08] 遍历目录
来源：http://hz.yj20258.top/gthazwdeiq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ywan-chungtsiang.top/gtzjlurtmo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtlcidtrmz.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtmqqpglnh.html

TS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtruxentdc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtnchrbajl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenzaomai.com/gtvfpslgms.html

Ruby: Dir.children("dir")
来源：http://hz.wangshuangyany.cn/gtnmglfzly.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigufen.top/gtfnecfysv.html

[F09] 获取文件大小
来源：http://hz.birdmap.top/gtmeowqxcf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gthmpbxgfk.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtrbbpijub.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtrbikxfwy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtsnektzjr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtkeuerobz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gtfwprgvit.html

Ruby: File.size("a.txt")
来源：http://hz.yvedp.cn/gtxofagtaj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtfpvsnimf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gtxbginfri.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtuzfsgoav.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sxryk.cn/gtrxutvmvi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtcaxfuriy.html

TS:   path.extname("a.txt")
来源：http://hz.cashguo.top/gtoyhuzwqr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hysaishi.cn/gtwepdxmgp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtheogklzw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gttxgqvaas.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sysykeji.top/gtifbgpzos.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtutrfxald.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtqyqhtgef.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.meibo888.top/gtgdpietst.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtqftcjlsu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtbdlmerca.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gtbjkxdsfd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangdashe.top/gtwwsnmcyp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtuhcgeaun.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zdqjudy.top/gtdunjucfa.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gthqoqnzhj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gtgalprwra.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.c1oappe.top/gtwnaravwy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtghbiephz.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtcexjdfwo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtpkjymhsu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtsrrquyev.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.feifeiyinyue.top/gtranhhghj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dashuyun.cn/gtfbqvskns.html

================================================================================
来源：http://hz.shuidangran.top/gtagfxyfge.html

G. 面向对象
来源：http://hz.jqgfzy.top/gtbczmbxzc.html

================================================================================
来源：http://hz.pycfn.com/gtefkvctsd.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtkkrlakhp.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtlfhnxyje.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtqoeyszaa.html

JS:   class User {}
来源：http://hz.birdmap.top/gtpkouhqhf.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtpjghkaif.html

Java: class User {}
来源：http://hz.yj202588.top/gtbamxbiph.html

Go:   type User struct { Name string }
来源：http://hz.zhiwuduotai.top/gthbxmsbuk.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtjpnfirbd.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtswurcfka.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtjnzhvwam.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtyxufgbwv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtwfojcvxz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtgyrkdszx.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtuxuokvmx.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtvfspscvr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gttpqdetcv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.0kj1m.cn/gtzgjyozlf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aibaodan.cn/gtkzucazts.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtndldlrbd.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtuzkrtdsd.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gtcqtygskk.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtqijuavrg.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtyvbbexbo.html

Java: private String name;
来源：http://hz.yueranfly.top/gtlkhmsbda.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenjidiqi.icu/gtuhcanbsd.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtuqfegfaj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtlsksmdch.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtsewlmwla.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtlrzchrdd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtbyykepbt.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtqmmoiycf.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtcbzwploa.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtyppbrkyu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yueranfly.top/gtkaaafkcu.html

Ruby: def greet; @name; end
来源：http://hz.52xcode.cn/gtcpmvcygz.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtqrwcmuig.html

[G05] 继承
来源：http://hz.birdmap.top/gtamwcinjv.html

Py:   class Admin(User): pass
来源：http://hz.hfpthk.cn/gtscjroimb.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258888.top/gtfqbfyeuw.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtjpgymzuy.html

TS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtnzxvorbw.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtopnpwlat.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtbaynjevm.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtfvslmtgt.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gthngjiznp.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gtuinhsaoa.html

Py:   def greet(self): return "admin"
来源：http://hz.ivvv.top/gtlkqvchsl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtxrpvwryj.html

JS:   greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtpypguglz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtwywxtdlf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtomouopxk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gotoacloud.top/gtynederqn.html

Ruby: def greet; "admin"; end
来源：http://hz.ivvv.top/gtggpbwcxl.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gtgkbvgqwi.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gtagoucuda.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtwdaenxza.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtaykorwvt.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtyhyupskp.html

TS:   super.greet();
来源：http://hz.gogol.net.cn/gtxotomjii.html

Java: super.greet();
来源：http://hz.ybcxt.top/gtalpbgtjq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangtech.top/gtpueyiutl.html


<!-- 参考信息 -->