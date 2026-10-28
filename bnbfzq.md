代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtggazzvsw.html

Java: String.format("%03d", 7)
来源：http://hz.yuanzhike.top/gtedsqblzb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cheryme.top/gtrgfuqgjl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shzxlz.cn/gtrppuksds.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtrwjyuzrf.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtqbfbjddm.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtzqqfxpoi.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtfbhcokue.html

JS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gteyefgezq.html

TS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtzbvnyoej.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenjidiqi.icu/gtfeedevgo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgufenzy.top/gtbcisuqfl.html

Ruby: s.reverse
来源：http://hz.jianghu66.top/gtxkivgdjt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtdwnewqtd.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gtsbeftvmr.html

Py:   s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtqncicyug.html

PHP:  substr_count($s, "a");
来源：http://hz.yuxming.cn/gtkasbijxe.html

JS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gtyrnczpab.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtnzplbufd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.316326.xyz/gttvrpkcvn.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtxnfqwxnr.html

Ruby: s.count("a")
来源：http://hz.yvedp.cn/gtjiwfjlbd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.mhx1999.top/gtljyvtykl.html

[E13] 逐字符遍历
来源：http://hz.sufxvd.cn/gtwzhpbwhg.html

Py:   for ch in s: print(ch)
来源：http://hz.aizwys.cn/gtedcpcasw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj202588.top/gtczfgwgzg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gthwggchne.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtclcuuqoh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cqqwz.cn/gtxcdojftb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gttlrgqcad.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.mhx1999.top/gtqjnvtcis.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuetiantiany.cn/gtgfapuptm.html

[E14] URL 编码与 Base64
来源：http://hz.yonumen.top/gtlkklfnbx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guowangkeji.top/gtomrngeym.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shuidangran.top/gtihjehbga.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gtesjztfkv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtkhjrqisk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tian-w.cn/gtbaqwqgxk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxuanxn.top/gtffiekldb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangshuangyany.cn/gtqmlmsjnz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gthiakoyjw.html

[E15] HTML 转义 / 反转义
来源：http://hz.9152youxi.cn/gtptkgibat.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuetiantiany.cn/gtkquwocvq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuanzhike.top/gtuxiyztkq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jyoumei.cn/gtzuakvsix.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinyuanbaomall.cn/gtjaezskvh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aizwys.cn/gtefccfyui.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yongpay.top/gtlovdkufq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sxryk.cn/gtlvsskygt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtcpumounl.html

[E16] 数字千分位
来源：http://hz.fzhhl.top/gtkbtsgetm.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtdnscuxmw.html

PHP:  number_format(1234567);
来源：http://hz.redwolf501.top/gtntepxrxs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtcobmlmqm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtpwpbtxub.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenzaomai.com/gturocxfiu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenlongwang.top/gtgtdatvqv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shuidangran.top/gtjiikzncq.html

C#:   1234567.ToString("N0")
来源：http://hz.yueranfly.top/gtprjqchps.html

[E17] 首字母大写
来源：http://hz.yvedp.cn/gtgsdtxpfv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtjbiajzbu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cdnleiting.top/gtvatynmae.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtlqyknfmh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtosnpuzih.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zycfv.cn/gtzeyocvsx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pengpengdd.cyou/gtaleyzbvt.html

Ruby: s.capitalize
来源：http://hz.tianlin.xyz/gtilbdngoz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.guannengcc.top/gtgijmegco.html

[E18] 模板占位符替换
来源：http://hz.snrcjt.cn/gtadknnvoz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtyaxyrknt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtdhleesqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtmkmcuxxj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtdqmrzdbi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.svipenyu.cn/gtnsdtimyr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gthxzhdtym.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtkzasfcwx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtmvzlxizs.html

[E19] 多行文本按行拆分
来源：http://hz.yangfankeji.com/gtvmuvoxtg.html

Py:   s.splitlines()
来源：http://hz.redwolf501.top/gtzzgwwxon.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dashuyun.cn/gtnhjkrdfq.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtfqixjdju.html

TS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtdzkhttkg.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gtsyvzamyw.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtfuisryvo.html

Ruby: s.lines
来源：http://hz.jinqigfzy.top/gtjkbqavvg.html

C#:   s.Split('\n')
来源：http://hz.chenjidiqi.icu/gtwglfyqpd.html

[E20] 判断字符串是否为空
来源：http://hz.tian-w.cn/gtfbcuvbse.html

Py:   if not s:
来源：http://hz.c1oappe.top/gtiqsxljqh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtiiyeoiwy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ehwqpu.com/gtcrrfjjrk.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtuqjgqxaz.html

Java: if (s.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtzzgmjele.html

Go:   if s == "" {}
来源：http://hz.aizwys.cn/gtdtzpiigt.html

Ruby: if s.empty?
来源：http://hz.gogol.net.cn/gtitpxkuek.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.iojbl.cn/gtaouavehn.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gttiiiroho.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtuuddfcco.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yongpay.top/gtkjbtzdaa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gthxojxalx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtlstozfmp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtcezjezfu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigufen.top/gtdevcsnuy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nwbrower.top/gtutolnsgu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cheryme.top/gtxeikdabv.html

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gtjzallkcv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuanzx.com/gtacvgyjym.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtlkokgcuw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gtajrwjhji.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtqjehxbhh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnqzz.top/gtfmbxfdci.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuetiantiany.cn/gtlerrqvwr.html

Ruby: s.bytesize;  s.length
来源：http://hz.tanke756.top/gtmkvdfwpr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jlsjyb.cn/gtdpkkpsfm.html

================================================================================
来源：http://hz.cqqwz.cn/gteihgwkaz.html

F. 文件与目录
来源：http://hz.jinqigufen.top/gthhtsuram.html

================================================================================
来源：http://hz.yvedp.cn/gtauhqofsi.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtnhftdxsa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.0kj1m.cn/gtzzdojzwi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gtpusmbpca.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtckgsgwcw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fengsongda.top/gtmsxxwvkw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gttggtdoim.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zycfv.cn/gtzqplkbkw.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtjydgczom.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.vqdsnc.cn/gtfzkbpbve.html

[F02] 逐行读取文件
来源：http://hz.zhijiandao.cn/gthbqurwqn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangkeji.top/gtgzxyeunw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuanzhike.top/gtolpbostg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.quarkkingdee.top/gtbiyuzryj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtrgzggsut.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtwacxmlkq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hongshengwenyu.top/gtemxtuhxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gogol.net.cn/gtnjtaakyr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gthayyhftm.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtchasdqno.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gtjcozthnz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtwcrzzhqx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtttmujcje.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gttyypoxft.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhengqikj.top/gtxyzbvyym.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gthaekwnvm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtmllbltcv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtlrudadoe.html

[F04] 追加写入文件
来源：http://hz.jqgufenzy.top/gtxwmoczcj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhaomingkeji.xyz/gtouulzhdp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtralkvffc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtekzmkkwy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtkwhyhoqs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtcvnrhody.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj202588.top/gtbmfbvtkg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.andypj.xyz/gttrlhwfll.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cheryme.top/gtcdjmapcr.html

[F05] 判断文件或目录是否存在
来源：http://hz.mhx1999.top/gtxsbaecuk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ivvv.top/gtycogfkki.html

PHP:  file_exists("a.txt");
来源：http://hz.ybcxt.top/gtddfxuaza.html

JS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtapgdggpk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtvmlxwnlz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtpebguzyk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yongpay.top/gttvkafocl.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gtpiqsnxfm.html

C#:   File.Exists("a.txt")
来源：http://hz.xinyue.icu/gtkkengbzt.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gtfzwwkhao.html

Py:   os.remove("a.txt")
来源：http://hz.jqgufenzy.top/gtrjldqnjq.html

PHP:  unlink("a.txt");
来源：http://hz.tianlin.xyz/gtghkecsqm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtpnduxrkx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtorudibst.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtskyoitoh.html

Go:   os.Remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtxjcjnlya.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gtlnpzzzsj.html

C#:   File.Delete("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtlevrwqdf.html

[F07] 创建目录（含多级）
来源：http://hz.xziqi.cn/gtholwlgpx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtovvcctsp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cheryme.top/gtnadzpihw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtizfzvdwd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtavhlclbw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtcocpzeny.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gtcndljthg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtywquorwz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.mhx1999.top/gtdkgwlxqv.html

[F08] 遍历目录
来源：http://hz.316326.xyz/gtwyulwyea.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daria6918.cn/gtycnlxftv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jyoumei.cn/gtmmnlhtas.html

JS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtzhsdmbde.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtpptcfglh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtocjuyduz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtlsmnorrl.html

Ruby: Dir.children("dir")
来源：http://hz.xinyue.icu/gthkkfvmjl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuxming.cn/gtocsbzebe.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtuyhjnzfl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gtlhcxdgbs.html

PHP:  filesize("a.txt");
来源：http://hz.hnqzz.top/gtjsewuxdl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtqnzxxrgx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtpkgovlxb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtycaiopye.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fengsongda.top/gtscaqmdwi.html

Ruby: File.size("a.txt")
来源：http://hz.tianlin.xyz/gtziggpwaw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtxfxgpzah.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxinkj.top/gtrjrjadkk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtwevsbahw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtipxcivhx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtrjbjwnde.html

TS:   path.extname("a.txt")
来源：http://hz.bjfxy.top/gtelaedtho.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuanzhike.top/gtbxsaizjd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtmyqcsdbp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtiupasfog.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gtgrbubqvf.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtqybzszmb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtadbklcwr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigfzy.top/gtdwzejpga.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtymdzbtqz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gteeqofglw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gogol.net.cn/gtleoclcdc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtxtuyydea.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gthqttrulf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.redwolf501.top/gtmlwocpfo.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtetsbbvwu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.bjfxy.top/gtmbibahjq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtpehtjrfc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.snrcjt.cn/gtpdhoibak.html

TS:   // 同上
来源：http://hz.ivvv.top/gtbhxgtkhj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gthtgkckva.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yueranfly.top/gtpadomknu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtnmzrrysp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yongpay.top/gtsdyopiui.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtiweqiwej.html

G. 面向对象
来源：http://hz.hfpthk.cn/gtsryjqgef.html

================================================================================
来源：http://hz.cqqwz.cn/gtigjhzcgd.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtrtefehxl.html

Py:   class User: pass
来源：http://hz.tianlin.xyz/gtokscmrox.html

PHP:  class User {}
来源：http://hz.fzhhl.top/gtqbawoxqc.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtfirtadwc.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtvryaddiv.html

Java: class User {}
来源：http://hz.fzhhl.top/gtsdlyqozo.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gtvomiiqck.html

Ruby: class User; end
来源：http://hz.mhx1999.top/gtckhpokib.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gtedmtfcbh.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtpnakqahj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gtqcxqpnwf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtklzcfqff.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj202588.top/gtoufxugiy.html

TS:   constructor(public name: string) {}
来源：http://hz.gogol.net.cn/gtthwjmyhj.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtqohfqoqx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangdashe.top/gtbqvvkgti.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ywan-chungtsiang.top/gtntdkwiiw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtiiepbipq.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtukskjtas.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtdosmonjm.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtutiwbefk.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gtimykuxlj.html

TS:   name: string = "x";
来源：http://hz.xinyue.icu/gttmpimweq.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtahxceapp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hysaishi.cn/gtjcwlgggu.html

Ruby: @name = "x"
来源：http://hz.zhengqikj.top/gtcjnnjdei.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jiagoushi.top/gtoexukjku.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gtzjwnijsc.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigfzy.top/gtuvnuzmos.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtrijvwrpr.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtmscxriab.html

TS:   greet(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtsljkczed.html

Java: String greet() { return name; }
来源：http://hz.kuanghao11.cn/gtkehjyaog.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtejsdgbzt.html

Ruby: def greet; @name; end
来源：http://hz.ybcxt.top/gthxncubhq.html

C#:   public string Greet() => Name;
来源：http://hz.chenlongwang.top/gtolyuylhv.html

[G05] 继承
来源：http://hz.gzhubu.top/gtqwpjioec.html

Py:   class Admin(User): pass
来源：http://hz.snrcjt.cn/gtawrfbufo.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtulueaifp.html

JS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtvaqpjmsz.html

TS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gthgqhwkcf.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gtqptwryvo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gtrbbzuvwx.html

Ruby: class Admin < User; end
来源：http://hz.guowangkeji.top/gtearhibkd.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gtgfymqicu.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gthhcoeycw.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gtbxkhbssv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtkiocfmdt.html

JS:   greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtobbihtfu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtlhdtyluh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtpwfioiok.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.haohaochexian.top/gtizmffkcn.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtnpwssnyk.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtlkpfffwi.html

[G07] 调用父类方法
来源：http://hz.jqgfzy.top/gtkbkydfid.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtgsqtzfjk.html

PHP:  parent::greet();
来源：http://hz.yj20258.top/gthfcmzmog.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gtnxyfhval.html

TS:   super.greet();
来源：http://hz.fzhhl.top/gtxixurbrh.html

Java: super.greet();
来源：http://hz.zdqjudy.top/gtplrrotrr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tianlin.xyz/gtzggzicsz.html

Ruby: super
来源：http://hz.0kj1m.cn/gtliievlqj.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtbslrtacg.html

[G08] 静态方法与属性
来源：http://hz.fzhhl.top/gthcveohgi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yangfankeji.com/gtvljvjoxk.html

PHP:  public static function f() {}
来源：http://hz.zhiwuduotai.top/gtgvawdazp.html

JS:   static f() {}
来源：http://hz.jinyuanbaomall.cn/gtywevmeka.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtzkzdjwtm.html

Java: static void f() {}
来源：http://hz.shanyushiyangkeji.top/gtsdfuarho.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnqzz.top/gtvssieibn.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtjhgrozxs.html

C#:   public static void F() {}
来源：http://hz.ivvv.top/gtwhpnecvh.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtsvxtorjg.html


<!-- 参考信息 -->