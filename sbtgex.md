代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.jlsjyb.cn/gttkmfeamh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gtmmkcoeko.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pycfn.com/gtpwjpcujx.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtuqejczjs.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtmtcvvmxr.html

Java: String.format("%03d", 7)
来源：http://hz.zhengqikj.top/gtmszhbshr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gtlmpsbvgx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gtghyigyee.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangdashe.top/gtfuvccaka.html

[E11] 反转字符串
来源：http://hz.guowangkeji.top/gtcsmllzwc.html

Py:   s[::-1]
来源：http://hz.hammf.cn/gttxqvkmpw.html

PHP:  strrev($s);
来源：http://hz.jiagoushi.top/gtgiiiyfbs.html

JS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtgopejmqr.html

TS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtcxqlawrh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtnkapqxfm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenzaomai.com/gthbhvvypo.html

Ruby: s.reverse
来源：http://hz.ybcxt.top/gtbwtjiuzu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtwucbadrv.html

[E12] 统计某字符出现次数
来源：http://hz.hammf.cn/gthqavncpk.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtcwatabxy.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtxaowphmq.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtneigijyj.html

TS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gtpmgwgagn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tian-w.cn/gtcrkkircn.html

Go:   strings.Count(s, "a")
来源：http://hz.pengpengdd.cyou/gtrvhukxav.html

Ruby: s.count("a")
来源：http://hz.zhengqikj.top/gtkvxojufl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtsjvybtjl.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtssnivokx.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gtsvkrhdwt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangtech.top/gtxrtcjfxn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtakobpmox.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtvondvuvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shzxlz.cn/gtmajseepq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtmhtasfyu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtuadzplpw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pengpengdd.cyou/gtlarpzbia.html

[E14] URL 编码与 Base64
来源：http://hz.iojbl.cn/gtpgowplaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtprvacrtq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gogol.net.cn/gtbwmydmci.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ydjk.org.cn/gtkezggjlq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuanzhike.top/gtxowzomoo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hysaishi.cn/gtczqgptkv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cashguo.top/gtphlrzgft.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hongshengwenyu.top/gtfnxjvmil.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtdtxfakhj.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtspwriyph.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangdashe.top/gtcmomxuzn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.c1oappe.top/gttityauze.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tianlin.xyz/gtsofkghsi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tianlin.xyz/gtazquvnpz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.havefunace.top/gtxtlwshsh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guannengcc.top/gtgowfqkfb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtfuigsaax.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hysaishi.cn/gtkhvpgahq.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtzgdarmxo.html

Py:   f"{1234567:,}"
来源：http://hz.xylfe.cn/gtwzmoqavf.html

PHP:  number_format(1234567);
来源：http://hz.gotoacloud.top/gthaissopj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtreckeikw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtyzjffozw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.svipenyu.cn/gtezhcdexg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtahkndzju.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gtldvjdtzk.html

C#:   1234567.ToString("N0")
来源：http://hz.chenlongwang.top/gtycvxpwdj.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtbvipzfhx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gtrcnjzcbl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj202588.top/gtdagwqmyy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangdashe.top/gtdyjcbbrb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtynfmbxhp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ywan-chungtsiang.top/gtabtwhefz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daria6918.cn/gtzwlmanxv.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtsimfcdrv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cashguo.top/gtmbrvklrc.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gtwlyvdwrp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dashuyun.cn/gtudrtxvpa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtrwjfbrcz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtqzcwnzhy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258888.top/gtuamkepye.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxinkj.top/gtvnlbbvfy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hywenlv.cn/gtxxbrpcej.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtuzxbptxk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gtorateszk.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtgqzwhptb.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtofqysfka.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtmvczrqfi.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtyuzddvsj.html

TS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gtshesrhlm.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gtudiveugs.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhoulong.xyz/gtvemubhqs.html

Ruby: s.lines
来源：http://hz.xingfuxueyuan.xyz/gtioqohykr.html

C#:   s.Split('\n')
来源：http://hz.yangfankeji.com/gtjjcypwkb.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtvclrpxpa.html

Py:   if not s:
来源：http://hz.316326.xyz/gtcllnfnse.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.redwolf501.top/gtgrssucuj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gtvcqyhlky.html

TS:   if (s === "") {}
来源：http://hz.svipenyu.cn/gtbbdlnifc.html

Java: if (s.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtjpzawlnb.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gtootmcfjz.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gtthyrqelh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hnxiangtu.top/gtweygokex.html

[E21] 超长截断加省略号
来源：http://hz.dashuyun.cn/gtqhtbutge.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cashguo.top/gtagvadzbk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.9152youxi.cn/gtptlbftkg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtxveykwlg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtdzeswihu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtudbvyujs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuxming.cn/gttotvbvpe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gteovegtnd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtqiqmoieh.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtjneitbzn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtkqulezeb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gthyoirlsn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtzqfeykxe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtcnjcvlkb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shzxlz.cn/gtghrbuxqe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigfzy.top/gtvhffrniw.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtctcprarr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gogol.net.cn/gtglmfdxpv.html

================================================================================
来源：http://hz.yj20258888.top/gtdwmrcuxg.html

F. 文件与目录
来源：http://hz.chenlongwang.top/gtdgbfdfrr.html

================================================================================
来源：http://hz.nanxinkj.top/gtkgimslhw.html

[F01] 读取整个文件
来源：http://hz.haohaochexian.top/gtswqpslve.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gotoacloud.top/gtdshqissp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gaohongyu789.top/gterrfoorn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.0kj1m.cn/gtcrearxme.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gotoacloud.top/gtxrefttej.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtkvuomhfo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shangyingyoupin.top/gttybkorjs.html

Ruby: File.read("a.txt")
来源：http://hz.birdmap.top/gtehpzkyxz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtkhynuajs.html

[F02] 逐行读取文件
来源：http://hz.bjfxy.top/gtisapnpvu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.bjfxy.top/gtghnnficr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dianchejie.cn/gtgpwigbdy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtncumfryv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtarlscscs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtgxasoacy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtzarrmstd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.kuanghao11.cn/gttvfdwzuv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtrlocdsir.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtzmvppjfa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtuldwjvkk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gthjjbtgwo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtotlrbtxp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtiadfsghf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.daxiang520.top/gthjxvujib.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gtczhnzsfb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258.top/gtjyfplxtv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gtvwklwdst.html

[F04] 追加写入文件
来源：http://hz.cheryme.top/gtkfkgvrzl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtdsqbunzm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jiagoushi.top/gtpxetxqxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtfdetxend.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtlmueegac.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gotoacloud.top/gtrfkipdqv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sweek.top/gtvssjidtl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jianghu66.top/gtvrfnhmwk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtktjfefnl.html

[F05] 判断文件或目录是否存在
来源：http://hz.52xcode.cn/gtxkgjqdti.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gtpazbrbfp.html

PHP:  file_exists("a.txt");
来源：http://hz.dashuyun.cn/gtjhtiutap.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gthzxvfnso.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtciljxkho.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gttkfecgcd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gtqxlykvnq.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgufenzy.top/gtjlguirkp.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtmebqdwyw.html

[F06] 删除文件
来源：http://hz.xinyue.icu/gtpkfyomgw.html

Py:   os.remove("a.txt")
来源：http://hz.shzxlz.cn/gtdquzliie.html

PHP:  unlink("a.txt");
来源：http://hz.hammf.cn/gtrvujawwh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtkrzehhsq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtnhdvtsur.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtylrmbzna.html

Go:   os.Remove("a.txt")
来源：http://hz.zhengqikj.top/gtycdsmlbw.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtnlovxhkd.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtchmyqdvv.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtxzkusqsm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yonumen.top/gtckwcarsu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtexzcltjg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtqjlbuxow.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gtpxmbxfca.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtvuexaibh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtxoofpsdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xingfuxueyuan.xyz/gtsektbjge.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhongyouzk.top/gtodwmloxe.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gtquaqhfqf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhoulong.xyz/gthfbkietb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shuidangran.top/gtlajwimyv.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gthiuvsoox.html

TS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtdhxndpls.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtieeutobc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.haohaochexian.top/gtdvvqdulv.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtwmngmuqm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtkzjfunjn.html

[F09] 获取文件大小
来源：http://hz.quarkkingdee.top/gtgwdgzkqw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenjidiqi.icu/gtkbnkzsvi.html

PHP:  filesize("a.txt");
来源：http://hz.yj202588.top/gtkwzjpdwv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtpmajaaje.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtsabjixzq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtmvkbdvdq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtjlfbvwfl.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtxwesimwj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pengpengdd.cyou/gtlnvcwxmv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ywan-chungtsiang.top/gtiwouhtvu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gthiapahav.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gzhubu.top/gtvhmoxtzr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtbtshqbym.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gteugmxkom.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shzxlz.cn/gtncghdhli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtbhhyiure.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtnbijopir.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258888.top/gtqaxvytoz.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gtcdefgwah.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtmoyniqnt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gtojzytfah.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtapohhiju.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtzbstjgbd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gtgdkxnmjo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.meibo888.top/gtozxrimjz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtlkiuzkra.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sweek.top/gtlusedrky.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtqouraxja.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtlzcsijfq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guannengcc.top/gtirukwmsl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ivvv.top/gtrgrlaqmj.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtktxwwhsa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtdfsdwdeu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtekgsblje.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sxryk.cn/gtopoxhnaw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtiujolfmr.html

================================================================================
来源：http://hz.svipenyu.cn/gtxxekuoph.html

G. 面向对象
来源：http://hz.jianghu66.top/gtcwcysxyn.html

================================================================================
来源：http://hz.xziqi.cn/gtjrhtfwqr.html

[G01] 定义类
来源：http://hz.zhixingplan.top/gtzdfonepd.html

Py:   class User: pass
来源：http://hz.andypj.xyz/gtrxkalmfp.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtqijtjrnr.html

JS:   class User {}
来源：http://hz.yvedp.cn/gtzveewlkr.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtxqwufxhe.html

Java: class User {}
来源：http://hz.gotoacloud.top/gtcontqcwa.html

Go:   type User struct { Name string }
来源：http://hz.jinqigfzy.top/gtgeuujfaa.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtqbhlawpr.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtecpvtbcx.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtblfablev.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtgivuewwa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtggjwqzwc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtcbxnsvqw.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtzdfrbuhy.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtwheqpqez.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtrnkrtmno.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yvedp.cn/gtuzfrnocl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fzhhl.top/gtyvhzavxg.html

[G03] 实例属性
来源：http://hz.zhiwuduotai.top/gtwyuzaahm.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtlwyibegn.html

PHP:  public string $name = "x";
来源：http://hz.ydjk.org.cn/gtdaccgblo.html

JS:   this.name = "x";
来源：http://hz.yj202588.top/gtomdmsapp.html

TS:   name: string = "x";
来源：http://hz.sxryk.cn/gtueslmbdc.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtmtzaeubk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtstkhiwwl.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtoczyjhna.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gtxqyhkxit.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gthzbeapeg.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtmxfdljwr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtvxbtkply.html

JS:   greet() { return this.name; }
来源：http://hz.ydjk.org.cn/gtmcqcwbgd.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtaibrvsbo.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtaeblqwvj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtiycxvfbv.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtbydlprms.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtoywnwezh.html

[G05] 继承
来源：http://hz.aizwys.cn/gttpqduvrn.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtxcglapdh.html

PHP:  class Admin extends User {}
来源：http://hz.cashguo.top/gtmlchqqvy.html

JS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtmxvxdqyh.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtylcdxhvx.html

Java: class Admin extends User {}
来源：http://hz.gotoacloud.top/gtwnwizerh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zdqjudy.top/gtpzinxbob.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gthykarqiv.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gthskinjrw.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtcqclyjbp.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtqesevegw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtynnjxgam.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtrzewatib.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtkrgjxmiw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtknvzwfda.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yongpay.top/gtaapwyqfd.html

Ruby: def greet; "admin"; end
来源：http://hz.hongshengwenyu.top/gtusjhznrk.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtegllmclz.html

[G07] 调用父类方法
来源：http://hz.nanxinkj.top/gtvahgyexy.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gthnkbgyqv.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gtxwduhufz.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtycjgriiq.html

TS:   super.greet();
来源：http://hz.aizwys.cn/gtpwrccvjj.html

Java: super.greet();
来源：http://hz.yonumen.top/gtmhbkjjsa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pycfn.com/gtvxevozyi.html

Ruby: super
来源：http://hz.sxryk.cn/gtiizpagtn.html

C#:   base.Greet();
来源：http://hz.jianghu66.top/gtfedpzsuf.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtquypzqow.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cheryme.top/gtfmmvhhog.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gtqwefmgpd.html

JS:   static f() {}
来源：http://hz.hfpthk.cn/gtovgtnlhl.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtidguikzs.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtibkvsrbb.html


<!-- 参考信息 -->