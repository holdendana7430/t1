代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hz.vqdsnc.cn/gtdncfuusr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.snrcjt.cn/gtqlpsayzf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigufen.top/gtgwguyoxi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuanzx.com/gtubiapcvc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtnzzfntrg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cashguo.top/gthgtudaql.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtghydfdpy.html

JS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtetnxqovm.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtmtrexmxv.html

Java: String.format("%03d", 7)
来源：http://hz.cdnleiting.top/gtweiutuqe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shzxlz.cn/gtdpacquzj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtonxazlvr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hfpthk.cn/gtfxuqyzdj.html

[E11] 反转字符串
来源：http://hz.ehwqpu.com/gthwiqujfi.html

Py:   s[::-1]
来源：http://hz.chenjidiqi.icu/gtladralti.html

PHP:  strrev($s);
来源：http://hz.redwolf501.top/gtizhekmyn.html

JS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtlgcrwzvv.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gttwcvshyv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenjidiqi.icu/gtihhpsvah.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gthatmopgn.html

Ruby: s.reverse
来源：http://hz.nanxinkj.top/gtgppwcuwd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gttqauvkgx.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtycqbefls.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtkffiypmy.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gtfwuszzzp.html

JS:   s.split("a").length - 1
来源：http://hz.hfpthk.cn/gtriydyjds.html

TS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtbutlymst.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtnhjtaboj.html

Go:   strings.Count(s, "a")
来源：http://hz.jianghu66.top/gtduokazew.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtkzhrutqj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fengsongda.top/gtowpobcqb.html

[E13] 逐字符遍历
来源：http://hz.hywenlv.cn/gtsvupznsz.html

Py:   for ch in s: print(ch)
来源：http://hz.zhoulong.xyz/gtczhprrxv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tianlin.xyz/gtfnxjnykx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtwsmxwydx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtoutfummd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sweek.top/gtuuzeinqi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.mhx1999.top/gtkaaicbyv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtyfghxevi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtiwmkoass.html

[E14] URL 编码与 Base64
来源：http://hz.sxryk.cn/gtqqrlpdft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.316326.xyz/gterapulmn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtvtrxrzmx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gtdwgqvuas.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gthgmbbbwe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtuemvvbzg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhixingplan.top/gteupshdaw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtwebygrbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.kuanghao11.cn/gtxgiqtogu.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenzaomai.com/gtmqcxlnen.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guannengcc.top/gtojdzrvdy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuxming.cn/gtjgekmctx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ywan-chungtsiang.top/gtgmeduqqk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pengpengdd.cyou/gtdplxdyqd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gterdqnlws.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangkeji.top/gtcavkfohf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtalaxsqtt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtjiofrvgi.html

[E16] 数字千分位
来源：http://hz.andypj.xyz/gtmgknjmsr.html

Py:   f"{1234567:,}"
来源：http://hz.yanxiufei.cn/gtcudkxtcf.html

PHP:  number_format(1234567);
来源：http://hz.sufxvd.cn/gtsnnhtajq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtkgkpnrtm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtvksquwad.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtjopbcycc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.vqdsnc.cn/gthrzomhta.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigufen.top/gtthakgevw.html

C#:   1234567.ToString("N0")
来源：http://hz.snrcjt.cn/gtsaoobggr.html

[E17] 首字母大写
来源：http://hz.gogol.net.cn/gtxcyvayzw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtjiwohumu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtvnenryic.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtcwbmfdkl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtulbplpck.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.svipenyu.cn/gtwxlaglgu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtshnzrkbs.html

Ruby: s.capitalize
来源：http://hz.ivvv.top/gtygqjfpet.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gzhubu.top/gtxnkcazdu.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtaapcgead.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtuzqdfpgz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhoulong.xyz/gtekblvvcs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtktpjxjct.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtvhltvtjh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gtflsactov.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtgpdexxed.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydjk.org.cn/gtaruenrru.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cucudq.cn/gtehxqbksg.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtlfmtqgtq.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtqcwakdvm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydjk.org.cn/gtipqstevr.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtxordijzv.html

TS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtmefqyviq.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtrgkjxsng.html

Go:   strings.Split(s, "\n")
来源：http://hz.316326.xyz/gtlvwgormx.html

Ruby: s.lines
来源：http://hz.ybcxt.top/gtcgaaosoz.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtmvjgvjnv.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtebvggxov.html

Py:   if not s:
来源：http://hz.daria6918.cn/gtgswmalhk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cashguo.top/gtbklzrmcv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gogol.net.cn/gtcqtdwsbf.html

TS:   if (s === "") {}
来源：http://hz.pycfn.com/gtqprsyjoj.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gthztowjuh.html

Go:   if s == "" {}
来源：http://hz.nanxinkj.top/gtcqzbwmfl.html

Ruby: if s.empty?
来源：http://hz.chenlongwang.top/gtafigjjtn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fengsongda.top/gtxmrvorqd.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtdbvenqgg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuxming.cn/gtupheayoy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tanke756.top/gtghegyllv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtrwosbfbt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtykuwmazi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtckhpixkx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtbtyobvnj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.andypj.xyz/gtkgxdopar.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtpulsolpm.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gtnohndcpb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ppjwa.cn/gthzplhtig.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtvcujlnht.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtewtknauf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtdflmfmvn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxinkj.top/gtuvcltaew.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ppjwa.cn/gtzvlmroyt.html

Ruby: s.bytesize;  s.length
来源：http://hz.vqdsnc.cn/gtznhanihz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zdqjudy.top/gtetoafviu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtytxdnqei.html

F. 文件与目录
来源：http://hz.bjfxy.top/gtecqxozfb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbffqlgsn.html

[F01] 读取整个文件
来源：http://hz.yuxming.cn/gtlesussbd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtxrarogdu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.316326.xyz/gtekmhwnue.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ivvv.top/gtkwxxdmqv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gttxdyvdse.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtsrouptet.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtxthkjqth.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangtech.top/gtywciykag.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtoddxqots.html

[F02] 逐行读取文件
来源：http://hz.shangyingyoupin.top/gtbkimozoe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cdnleiting.top/gtyrwwepsd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtqpzecsud.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtazlfadbe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtwjizteuf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sweek.top/gterutpagd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtnvjoxpyv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangtech.top/gtxdssgnlc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtenwrclxw.html

[F03] 写入文件（覆盖）
来源：http://hz.feifeiyinyue.top/gtylfssldn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtnyidfhxh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.iojbl.cn/gtorpotrzv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtyxggneyh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtdcemaftj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhiwuduotai.top/gtulfroepj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.316326.xyz/gtzvttvunm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtkhxdttlt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtnlppaqqq.html

[F04] 追加写入文件
来源：http://hz.c1oappe.top/gtesebjkkd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hongshengwenyu.top/gtieikrvkx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydjk.org.cn/gtsfhxpgno.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtvsuhmcky.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtbpdjmahu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hfpthk.cn/gtblovdtia.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gaohongyu789.top/gtcpmwmutl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenzaomai.com/gtrybmwrmg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigfzy.top/gttxfpwect.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuxming.cn/gtmjkqojsa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtretllhgo.html

PHP:  file_exists("a.txt");
来源：http://hz.daxiang520.top/gtunviucnb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gttwektqdd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtfqnjyyrf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtwpmduoro.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinyuanbaomall.cn/gtywdnwkqp.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtvxtwnvus.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gtmmqcxhzm.html

[F06] 删除文件
来源：http://hz.ybcxt.top/gthqgehtgm.html

Py:   os.remove("a.txt")
来源：http://hz.ybcxt.top/gtcqrpaxsn.html

PHP:  unlink("a.txt");
来源：http://hz.guannengcc.top/gtdgemlhot.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtonlovxeh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtpcmcauad.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtgnxomovn.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtghddstiw.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtfsiitkef.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtyryyvfde.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtvypucsrd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangdashe.top/gtzewhojsb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yonumen.top/gtsvbxopds.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtecshltie.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtytfuulfo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtthackiar.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guowangkeji.top/gtuqzscits.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gtztttvpan.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.quarkkingdee.top/gtlpirpwet.html

[F08] 遍历目录
来源：http://hz.daria6918.cn/gtelehkjkv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sufxvd.cn/gtmtgrrwzv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhaomingkeji.xyz/gtaxzdqlou.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtpgyxrlvx.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtlbujgish.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtyvodjzgh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xylfe.cn/gtmxdbrjqt.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtbvuqyvse.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtgserramv.html

[F09] 获取文件大小
来源：http://hz.haohaochexian.top/gtdsephzrw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yonumen.top/gtflzwqsmb.html

PHP:  filesize("a.txt");
来源：http://hz.yuxming.cn/gtbybcbbey.html

JS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtvoyignzu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtyrvfffoy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gthheeupjk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtxwxrjeud.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gtuebvqvbi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtekjekvof.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtgvnslbuq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtmubiicri.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuetiantiany.cn/gttaovksox.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtjmauqtlh.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtfvjzoqzg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guannengcc.top/gtvkajpyry.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258888.top/gtaidnedvg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtmppstqix.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtdlvdklgm.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtbnilnkni.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtfbgwhpqr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gzhubu.top/gtglqthxmy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtvbacsfhr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gthkbscepw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtehgwizwm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtusbatubt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtytqxxxct.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.quarkkingdee.top/gtqswtahym.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtzqwfnokg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuanzhike.top/gtwvrscmca.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gtmmcwkftb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ywan-chungtsiang.top/gtdymbuftf.html

TS:   // 同上
来源：http://hz.havefunace.top/gtuqqwmyfg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.havefunace.top/gtfqjyzjsf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtoeufliwy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hfpthk.cn/gtypotakht.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtznjmfiar.html

================================================================================
来源：http://hz.hywenlv.cn/gtdmxtsbjt.html

G. 面向对象
来源：http://hz.316326.xyz/gtlroyvjjg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlheijrvo.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtocdgorig.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gtbbhghgnj.html

PHP:  class User {}
来源：http://hz.zhiwuduotai.top/gtxuadyolb.html

JS:   class User {}
来源：http://hz.yonumen.top/gtcnesshbn.html

TS:   class User { name: string = ""; }
来源：http://hz.hywenlv.cn/gthotlnzqn.html

Java: class User {}
来源：http://hz.ydjk.org.cn/gtjfrcjoqp.html

Go:   type User struct { Name string }
来源：http://hz.gotoacloud.top/gtpevowyup.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gttehgonki.html

C#:   class User {}
来源：http://hz.xuanzx.com/gtrmlhpwgf.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtijmgxmwq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sysykeji.top/gtsoenjnpp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtvvqsqrxj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtoyiadppm.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtjzltwcfp.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtcbzeankk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtgqtzwxan.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jiagoushi.top/gtzyyuyiyw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.vqdsnc.cn/gtsfsxvogk.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtklbdxxne.html

Py:   self.name = "x"
来源：http://hz.cqqwz.cn/gtodemohbb.html

PHP:  public string $name = "x";
来源：http://hz.zhongyouzk.top/gtuodpkdkk.html

JS:   this.name = "x";
来源：http://hz.hongshengwenyu.top/gtoosjndik.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtwwnyiapv.html

Java: private String name;
来源：http://hz.yanxiufei.cn/gtfvxzrrmm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtbmhoowki.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtauefirpi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigfzy.top/gtxwifryxl.html

[G04] 定义方法
来源：http://hz.nanxuanxn.top/gtzdzihbhu.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtkfoooonl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtznzlmtpa.html

JS:   greet() { return this.name; }
来源：http://hz.tanke756.top/gtsvuxnars.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtsaukrzal.html

Java: String greet() { return name; }
来源：http://hz.haohaochexian.top/gtuaatrqjn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yueranfly.top/gtaukgvtvc.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtspghqxyt.html

C#:   public string Greet() => Name;
来源：http://hz.feifeiyinyue.top/gtjjxkcxic.html

[G05] 继承
来源：http://hz.cashguo.top/gtxkzmvhyo.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtkzfaplyl.html

PHP:  class Admin extends User {}
来源：http://hz.yongpay.top/gtxrzhqzcp.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtotkagfgc.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtdlanhxba.html

Java: class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtujkbgswh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yonumen.top/gtcpwowfjd.html

Ruby: class Admin < User; end
来源：http://hz.wangdashe.top/gtdqrcxlfh.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtricpdcet.html

[G06] 重写方法
来源：http://hz.xinyue.icu/gttjzjuije.html

Py:   def greet(self): return "admin"
来源：http://hz.hnqzz.top/gtgcfabqsq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtsmzcnahs.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtgcdwphqh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtzctgyplq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtpqwoaozt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gthhsjrara.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtvrchtoic.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigfzy.top/gtinnoilzz.html

[G07] 调用父类方法
来源：http://hz.daxiang520.top/gtugpoczcn.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtxinonpif.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtjtcfrcjy.html

JS:   super.greet();
来源：http://hz.cdnleiting.top/gtzftdkxdr.html

TS:   super.greet();
来源：http://hz.sweek.top/gthjozuczx.html

Java: super.greet();
来源：http://hz.hysaishi.cn/gtlhynwzit.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gttydbdbvs.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtfvyrwlud.html

C#:   base.Greet();
来源：http://hz.zhongyouzk.top/gtsapiuchb.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtnxxnnlmr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.haohaochexian.top/gtcnybbcwr.html


<!-- 参考信息 -->