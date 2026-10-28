代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.shuidangran.top/gtldjlidec.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gtjsxpoqwb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.haohaochexian.top/gtcjsdnsco.html

JS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtpwfqkziy.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtkqawrjlg.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtcqkmdxtf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinqigfzy.top/gtjmkklexf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.andypj.xyz/gtpyobgyai.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shuidangran.top/gtpblvkjls.html

[E11] 反转字符串
来源：http://hz.pengpengdd.cyou/gtlfznnczz.html

Py:   s[::-1]
来源：http://hz.0kj1m.cn/gtstwaxhtr.html

PHP:  strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtysholexv.html

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtnxhqkcos.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtfkfzekpl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.pycfn.com/gtiksjzqiv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.316326.xyz/gthtbxsmcp.html

Ruby: s.reverse
来源：http://hz.zhixingplan.top/gtbyfewonw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtqagtauxz.html

[E12] 统计某字符出现次数
来源：http://hz.zhaomingkeji.xyz/gtnburulgu.html

Py:   s.count("a")
来源：http://hz.daxiang520.top/gtbwkkkzsi.html

PHP:  substr_count($s, "a");
来源：http://hz.ppjwa.cn/gtshjzbbqh.html

JS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtlzjfmxze.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtidtmhwfj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gttqhvzbdj.html

Go:   strings.Count(s, "a")
来源：http://hz.ehwqpu.com/gttpgawqnt.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtumvjaozx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dianchejie.cn/gtdtfwtgnr.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtxbbmiwlo.html

Py:   for ch in s: print(ch)
来源：http://hz.ydjk.org.cn/gtutbyimer.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtpoyqfvjh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtycsrqkwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtwqqwswed.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.meibo888.top/gtondrkaih.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj202588.top/gtkfniolum.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtvllsrixk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtmlhtscws.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtqbpjngne.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gaohongyu789.top/gteryaysxk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuanzx.com/gtfohoozpj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtrjuypsih.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuanzhike.top/gtodkzriiz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.316326.xyz/gtfzfwdzyn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gtdsufhspv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.birdmap.top/gtptfzrugf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.feifeiyinyue.top/gtnqubfotn.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtktogakkd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yanxiufei.cn/gtpqqqahlr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cdnleiting.top/gttbyfoxqg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fengsongda.top/gtvydinkdk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sufxvd.cn/gtcceizbkn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shzxlz.cn/gtkykemzuu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtxifrstqh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtinbnqkzq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gttadkrauq.html

[E16] 数字千分位
来源：http://hz.jyoumei.cn/gtydccymcw.html

Py:   f"{1234567:,}"
来源：http://hz.ydzc1.top/gtsrhzxnqc.html

PHP:  number_format(1234567);
来源：http://hz.cashguo.top/gtotswxkpl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtrdvxmevh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtmsxcpono.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.kuanghao11.cn/gtnwopaoiz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.316326.xyz/gttuqprcgz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtotegvpil.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gtrczvjwis.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtbvmxvihv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guannengcc.top/gttnkimoqr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.9152youxi.cn/gtfypomjfe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtbfkypdsj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtrdjpmieb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtygbnvuwj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hfpthk.cn/gtjybwgoyz.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gttekqffns.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtnmdjtzsf.html

[E18] 模板占位符替换
来源：http://hz.quarkkingdee.top/gtrmucgjng.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gtbthqjohf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xinyue.icu/gtczvhbdvs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtxgtjlexu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtuhpydbad.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shuidangran.top/gtmovypsvl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yongpay.top/gtdvxspaen.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fzhhl.top/gtftwgsvtb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.316326.xyz/gtxyzrbbhb.html

[E19] 多行文本按行拆分
来源：http://hz.haohaochexian.top/gtpbyjmlgg.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtjhpzsrwb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aizwys.cn/gtghjpknga.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtaiwhzagd.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtyooijszx.html

Java: s.lines().toList()
来源：http://hz.gaohongyu789.top/gtffdmkgph.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtzkyivxiv.html

Ruby: s.lines
来源：http://hz.yuanzhike.top/gtakvplwvc.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtecqeoerl.html

[E20] 判断字符串是否为空
来源：http://hz.jinyuanbaomall.cn/gtvxkkduzs.html

Py:   if not s:
来源：http://hz.xuanzx.com/gtivuhfajz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.havefunace.top/gteicwqfhl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jlsjyb.cn/gtpwptxdcq.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtlzabenzl.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtctjnvezf.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtoihrepup.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gturmehzgy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gtbyuwznfd.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtybhsoxsz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhixingplan.top/gtbnbfcodz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guannengcc.top/gtuhyomgej.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtriafvltk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtcrczmhel.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtmmxxnblz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtlwktyzze.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtmrjwqvnz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtxkrcenly.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gtkqulwsxc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fzhhl.top/gtmfqzytdl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtztdcnnih.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtcbviyxzv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtdppudexr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtrjusekrz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.feifeiyinyue.top/gtqrgghzva.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuanzx.com/gtocjshcno.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtraotitxl.html

================================================================================
来源：http://hz.yj20258.top/gtlzdwvakl.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtfyfrfdtb.html

================================================================================
来源：http://hz.jiagoushi.top/gtsyuzthxp.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtapqsepfy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtlbvhvmjo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxinkj.top/gtjcqyjljk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhijiandao.cn/gtudslrxpk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cheryme.top/gtlvlqseiv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtohgdaurt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenjidiqi.icu/gtfgjoompp.html

Ruby: File.read("a.txt")
来源：http://hz.gzhubu.top/gtxkasyewm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtpjkefygl.html

[F02] 逐行读取文件
来源：http://hz.gotoacloud.top/gttwqhfdvs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gtpnckakdv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtvyvlptbu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtnyccqtpl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gthukioosa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtjjlezohj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hywenlv.cn/gtyvjwjvfz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.0kj1m.cn/gtphguajzl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtqxzzwlxx.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtrcbleyiv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgufenzy.top/gtssrljwwc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zycfv.cn/gtktfezjoo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtisadipye.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtrkvmukth.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yj202588.top/gtjetfmhon.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.vqdsnc.cn/gtjzkwqfjp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhixingplan.top/gtjuwgoqrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.smart0.xyz/gtuixcijyv.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtdvuywlyb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtdetehkmf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtoclblgmo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtcydwxzwo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtjqmomdjv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtfsflrztb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtxidlcyht.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigfzy.top/gtbothhyee.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtcgtsnvtu.html

[F05] 判断文件或目录是否存在
来源：http://hz.snrcjt.cn/gtcofwqxua.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtfojeacyx.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtpgsbvurd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtgkfimnfo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtmrkyonhp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtqzcdcwny.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhongyouzk.top/gtgdrngzdj.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtkqbhchka.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gtwfsoieuu.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtrjtfjpcl.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtrwzvtlfd.html

PHP:  unlink("a.txt");
来源：http://hz.tian-w.cn/gttpiyhzin.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtowtihust.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtbraqaaiv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtdaqjpvrt.html

Go:   os.Remove("a.txt")
来源：http://hz.ydjk.org.cn/gtgfakqqmx.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gtcyimlsjn.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gthnhzupme.html

[F07] 创建目录（含多级）
来源：http://hz.zhijiandao.cn/gteklewxlx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnqzz.top/gtzqagmeld.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.316326.xyz/gtuhknapmf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtwppxcpge.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtlwsdzanm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gtqgefyzyh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.c1oappe.top/gtjxvgdhrq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tianlin.xyz/gtzuyvvjrk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtgowcgbwj.html

[F08] 遍历目录
来源：http://hz.ybcxt.top/gtdwldxohq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guowangkeji.top/gtzbrlwpyi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ivvv.top/gtakhzaegb.html

JS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gttxblqgng.html

TS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtfbkriaii.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtzgygqhol.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.iojbl.cn/gtzysifxfq.html

Ruby: Dir.children("dir")
来源：http://hz.yuanzhike.top/gtjetwsbfq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtujjclszr.html

[F09] 获取文件大小
来源：http://hz.jqgfzy.top/gtovzhqzss.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtjhhpvbal.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtridxgqbs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtraojzzcv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtykqjvpnn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtocujcgtd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenlongwang.top/gtksljofed.html

Ruby: File.size("a.txt")
来源：http://hz.yj202588.top/gtegbxapnk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shangyingyoupin.top/gtarqfxotz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtqgtlokmp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtuovouune.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daxiang520.top/gtzcicxguw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gthxeljyaj.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtxmitnwlv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtzgqyoeml.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtustnmhzc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtlgfnogcg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtsbbmfcoc.html

[F11] 复制与移动文件
来源：http://hz.jinqigufen.top/gtqodfoafe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtyywkogpz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtepmwoesc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtcnmktbbb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtxdplikvz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangshuangyany.cn/gtghylyujg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fengsongda.top/gtlvcelzam.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtnjbihpdh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gtgcxagwvm.html

[F12] CSV 读写
来源：http://hz.daria6918.cn/gtowznsnov.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtxpdtoire.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zycfv.cn/gtgdmhhcpk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtvyiuvqlf.html

TS:   // 同上
来源：http://hz.meibo888.top/gtemyyuoii.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtjhomhphb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xingfuxueyuan.xyz/gtiedtjciu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtizbgneii.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hnxiangtu.top/gtkeyjfidb.html

================================================================================
来源：http://hz.yuanzhike.top/gtphsgnibw.html

G. 面向对象
来源：http://hz.pengpengdd.cyou/gtoyqtmevu.html

================================================================================
来源：http://hz.cheryme.top/gtzbzayhri.html

[G01] 定义类
来源：http://hz.mhx1999.top/gtwvugrwha.html

Py:   class User: pass
来源：http://hz.sweek.top/gtutgvnnls.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtoepvadqf.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gttfielive.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gtguglbxia.html

Java: class User {}
来源：http://hz.yj20258.top/gtlehhwinj.html

Go:   type User struct { Name string }
来源：http://hz.xuanzx.com/gtpwvtxqlx.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtjjfytnun.html

C#:   class User {}
来源：http://hz.zhijiandao.cn/gtszwefzao.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtdipqnwhd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shuidangran.top/gtirltetkr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtpidymqqz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtuouzmyru.html

TS:   constructor(public name: string) {}
来源：http://hz.cucudq.cn/gtzfonigpf.html

Java: User(String name) { this.name = name; }
来源：http://hz.xinyue.icu/gtqfghjlrv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.vqdsnc.cn/gtpowaomjg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.andypj.xyz/gtveldwkex.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtkdnurpna.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gtzmrawbbv.html

Py:   self.name = "x"
来源：http://hz.feifeiyinyue.top/gtcfqzrhbx.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gttcrblysd.html

JS:   this.name = "x";
来源：http://hz.hammf.cn/gtozhoolbw.html

TS:   name: string = "x";
来源：http://hz.0kj1m.cn/gtfeqtjafi.html

Java: private String name;
来源：http://hz.smart0.xyz/gtriblwxip.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtdjvlovio.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtkhjiieir.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenzaomai.com/gtrhqxopzj.html

[G04] 定义方法
来源：http://hz.quarkkingdee.top/gtzxgciqln.html

Py:   def greet(self): return self.name
来源：http://hz.nwbrower.top/gtqyrzdbvq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtbisjrnpd.html

JS:   greet() { return this.name; }
来源：http://hz.cheryme.top/gtmzsutrix.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtzaligybt.html

Java: String greet() { return name; }
来源：http://hz.ydzc1.top/gtqrlzzknz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtnqvhagdt.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtcacizvgh.html

C#:   public string Greet() => Name;
来源：http://hz.fengsongda.top/gtawqddnue.html

[G05] 继承
来源：http://hz.cashguo.top/gteqddrdtg.html

Py:   class Admin(User): pass
来源：http://hz.zdqjudy.top/gtklgzrhbr.html

PHP:  class Admin extends User {}
来源：http://hz.zhengqikj.top/gtrtuoodpo.html

JS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtckgzvaup.html

TS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtxivikcib.html

Java: class Admin extends User {}
来源：http://hz.0kj1m.cn/gtptzfksbe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pycfn.com/gtgfphtcho.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtdudqcngr.html

C#:   class Admin : User {}
来源：http://hz.sweek.top/gthyywbxfl.html

[G06] 重写方法
来源：http://hz.9152youxi.cn/gtxcbfvill.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangkeji.top/gtkrkabjex.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtmeisgjit.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtdsxmunoh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtoyddhyqt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtqzrcxsnm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinyuanbaomall.cn/gtpmkwocaq.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtlajcuplc.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangtech.top/gthzdwpxan.html

[G07] 调用父类方法
来源：http://hz.9152youxi.cn/gtnsfwcpkd.html

Py:   super().greet()
来源：http://hz.cqqwz.cn/gtuxfouper.html

PHP:  parent::greet();
来源：http://hz.chenzaomai.com/gtvxnlzbwt.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtbdtixjnt.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtemjbjcvt.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gtjjyzambs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhijiandao.cn/gtyjwwjfkh.html

Ruby: super
来源：http://hz.sweek.top/gtafqgboaa.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtzovvxglh.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtapxrykgx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.andypj.xyz/gttfpaunvr.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtmcywltfv.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtcllpneqn.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtpsluween.html

Java: static void f() {}
来源：http://hz.hysaishi.cn/gtvlnrozpr.html


<!-- 参考信息 -->