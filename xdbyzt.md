代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cheryme.top/gtjuxzdrhb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtyojvxhvt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtszbkrgfg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gthlkadgoi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtawubxhgh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.quarkkingdee.top/gtpxkdzpbf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gtzmsucrtz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhengqikj.top/gttdbweanm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxinkj.top/gtfuzmvkwa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnqzz.top/gtbxjsrkxy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtrdgpdneb.html

JS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtlkrpbars.html

TS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtyxvzfeyk.html

Java: String.format("%03d", 7)
来源：http://hz.daria6918.cn/gtqgulfbvc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cheryme.top/gtclqypmhm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtdizujltx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtxjwlpprh.html

[E11] 反转字符串
来源：http://hz.bjfxy.top/gtislntpxd.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gtorpwppts.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtpxzfizom.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtykttqavj.html

TS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtilxceqrr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fzhhl.top/gtcaowdtij.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtmrahjjcn.html

Ruby: s.reverse
来源：http://hz.birdmap.top/gtleobjpqs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtflezkmvt.html

[E12] 统计某字符出现次数
来源：http://hz.zhiwuduotai.top/gtdowofvub.html

Py:   s.count("a")
来源：http://hz.9152youxi.cn/gthcpidlqf.html

PHP:  substr_count($s, "a");
来源：http://hz.zhongyouzk.top/gtbesauxeh.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtzkeukgcd.html

TS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtyldvtkol.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gteejxgoem.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtkjywpyvi.html

Ruby: s.count("a")
来源：http://hz.dianchejie.cn/gtaxmhciiq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtlkloueap.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gtpqzcsqpo.html

Py:   for ch in s: print(ch)
来源：http://hz.aibaodan.cn/gtsyvbnumm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xingfuxueyuan.xyz/gtloqulgto.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ybcxt.top/gtfnyyoipq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtwrflhkjr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.snrcjt.cn/gtxnpzmtcc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.haohaochexian.top/gtzfulxvex.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.0kj1m.cn/gtbdyfkngx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jyoumei.cn/gtqsmpthky.html

[E14] URL 编码与 Base64
来源：http://hz.zycfv.cn/gtgnflelks.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtswuewenm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtsventntj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtfyzkbgcf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gtyvjujnco.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtgvuetunl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtyslgxqwx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtyyxzmzly.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtjlbcqirw.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gtabfbyajs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pycfn.com/gtvpkcmnio.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigufen.top/gtbxqeczku.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.snrcjt.cn/gtnbtpwjni.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenzaomai.com/gttnpnnpar.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangdashe.top/gtmqpeaezc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sufxvd.cn/gtypdovmdd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtxnliahzc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tian-w.cn/gtpxdmfeee.html

[E16] 数字千分位
来源：http://hz.smart0.xyz/gthxutcmaa.html

Py:   f"{1234567:,}"
来源：http://hz.kuanghao11.cn/gtlyyjwrre.html

PHP:  number_format(1234567);
来源：http://hz.zhongyouzk.top/gtapptcjdo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtguqpjfaq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtutalybbu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.c1oappe.top/gtodkrrxmc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhixingplan.top/gtmfzzhpmo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gtnzjiqktd.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258.top/gtdwpdgvzx.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtoxwwpxuo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xylfe.cn/gtydzjcnag.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cqqwz.cn/gtfzixabqd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gtdvyfqxxd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtidyfiyla.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenzaomai.com/gtlxxkxlbo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gtotuqjxca.html

Ruby: s.capitalize
来源：http://hz.jinghuilouyu.cn/gtrekfqvmn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tanke756.top/gtqrwiqsum.html

[E18] 模板占位符替换
来源：http://hz.ydzc1.top/gtztuciwlx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhaomingkeji.xyz/gtbswjtyru.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtxsdqmveb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gttudesije.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtvzhvjkxg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hywenlv.cn/gtrychioxs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cashguo.top/gtwgrkggnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnqzz.top/gtxzgvosga.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yangfankeji.com/gtkushqhdj.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gteedvrtva.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gtywvrgkmy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnqzz.top/gtjiqkcqst.html

JS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtptvwfttl.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtnfwupvue.html

Java: s.lines().toList()
来源：http://hz.sxryk.cn/gthhimpmvw.html

Go:   strings.Split(s, "\n")
来源：http://hz.yvedp.cn/gtnburhlxl.html

Ruby: s.lines
来源：http://hz.guannengcc.top/gtmisqlgng.html

C#:   s.Split('\n')
来源：http://hz.cashguo.top/gtfloaezxf.html

[E20] 判断字符串是否为空
来源：http://hz.ydjk.org.cn/gttdudqbxs.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtgxfekwkc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.redwolf501.top/gthbxkhbiy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxuanxn.top/gtxytycbaq.html

TS:   if (s === "") {}
来源：http://hz.jinqigufen.top/gtiualkfir.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gthdkespkl.html

Go:   if s == "" {}
来源：http://hz.ivvv.top/gthkqcxkft.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtqphybnvk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sxryk.cn/gtjwzumlkv.html

[E21] 超长截断加省略号
来源：http://hz.iojbl.cn/gtdlzubwhg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtqtwwerda.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtrrcuwfkz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtqyyavskw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtrrqveswc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtxdbwygng.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gtmbbzulop.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhixingplan.top/gtltmqpstg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtvxoorgda.html

[E22] 字节长度与字符长度
来源：http://hz.zhiwuduotai.top/gtvqipotrx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnxiangtu.top/gtmsbtbvdk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtpcltyuqe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gthlaxjmmw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtatofvmhb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhoulong.xyz/gtzpltxbsm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aizwys.cn/gtovymbzmf.html

Ruby: s.bytesize;  s.length
来源：http://hz.cheryme.top/gtffbiprja.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aibaodan.cn/gtudmkctmh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzkbzqrdm.html

F. 文件与目录
来源：http://hz.aizwys.cn/gtftieabeq.html

================================================================================
来源：http://hz.xinyue.icu/gthfjupqdk.html

[F01] 读取整个文件
来源：http://hz.mhx1999.top/gtgtaesqcy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnxiangtu.top/gtkpiayvlt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aibaodan.cn/gtmemktnug.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gtsuclipma.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtfdgfxycf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtiqhhpzxl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ywan-chungtsiang.top/gtjuoiqefe.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtpxoobegf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtonjrzkcf.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtlmlzkjqx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.smart0.xyz/gtwgcsuywf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtgeqqacoy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtankigtzn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtozuzttgp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtqcsymewa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuxming.cn/gttegjrway.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hysaishi.cn/gtdmdwtbqa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtbwelztxn.html

[F03] 写入文件（覆盖）
来源：http://hz.nwbrower.top/gthcwsgxgm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xinyue.icu/gtsvrilrss.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.52xcode.cn/gtislgbpnu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtmepdveyy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtqzxlwthl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtgogsgfry.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtptyqnruv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sysykeji.top/gtenbaefxi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtvcwetaja.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtonrdvzoy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shuidangran.top/gtnktcfvri.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sysykeji.top/gtoxgebkwz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtqvoqvvey.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.havefunace.top/gtgxmgcgyy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.andypj.xyz/gtzzgoiezv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gtsujqrozj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtezqqqrag.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtolifwemt.html

[F05] 判断文件或目录是否存在
来源：http://hz.sysykeji.top/gtbtxivjzy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtnukjtdyq.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtzghcjftg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.0kj1m.cn/gtjgrvzxfh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtjuobxumr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtkmqcexov.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuanzx.com/gtqdghmvgp.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuetiantiany.cn/gtlzhyutqx.html

C#:   File.Exists("a.txt")
来源：http://hz.xziqi.cn/gtgcblvmyb.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtdvuefzrq.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258888.top/gtarfrzlwr.html

PHP:  unlink("a.txt");
来源：http://hz.snrcjt.cn/gtnhlcuwke.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtilrewtfs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtosyozxpd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtrluetibh.html

Go:   os.Remove("a.txt")
来源：http://hz.yanxiufei.cn/gtbqefykbz.html

Ruby: File.delete("a.txt")
来源：http://hz.jqgfzy.top/gtwwnwjshd.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtzdumsryv.html

[F07] 创建目录（含多级）
来源：http://hz.sxryk.cn/gtpxwhwolb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtnztynoxt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.0kj1m.cn/gtozpnwleo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtbdodjfax.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtdqpppcep.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gthucsyfio.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtfgbhtvhv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtwstdsuhd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gtxydzalol.html

[F08] 遍历目录
来源：http://hz.havefunace.top/gtbxhytarf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydzc1.top/gtslttfxep.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtucpcjmww.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtfgtnfhjz.html

TS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtdvvhtloo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtueecocxh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.iojbl.cn/gtrpoeuziq.html

Ruby: Dir.children("dir")
来源：http://hz.ydzc1.top/gtpljfseny.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhijiandao.cn/gtcbyfdqey.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gteibvprpb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.snrcjt.cn/gtfqcvbupa.html

PHP:  filesize("a.txt");
来源：http://hz.mhx1999.top/gtquicszcd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtiinjonju.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtmbrwwqcn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtxfixofmx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gotoacloud.top/gtstmflndl.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtalcvanru.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtqbpuhjcb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xingfuxueyuan.xyz/gtjueqmusq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtzkozavrm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gtqxurmiwl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtykdhgarl.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gtbgtigqzn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtxmeolwdo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.andypj.xyz/gtknnkdolp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtitpqkmli.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gteyzbgqug.html

[F11] 复制与移动文件
来源：http://hz.sweek.top/gtfnurytig.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtedhybtul.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtdrhccpkb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtnhvlwjwt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtcscvsonn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.mhx1999.top/gtjuszbbvy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtrpjdduuz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtdiaghcla.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtedueifub.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtibljucwz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtdcopdliu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtnrtuypzd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangkeji.top/gtmsfjnozz.html

TS:   // 同上
来源：http://hz.ivvv.top/gtoyrujtlb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.c1oappe.top/gtwngorpcj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hfpthk.cn/gtiowdryus.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.52xcode.cn/gtmkwxpnbh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.birdmap.top/gtmwufacxb.html

================================================================================
来源：http://hz.hywenlv.cn/gtagcbmuni.html

G. 面向对象
来源：http://hz.ivvv.top/gtcfauiiqi.html

================================================================================
来源：http://hz.cdnleiting.top/gtzwhsoije.html

[G01] 定义类
来源：http://hz.smart0.xyz/gthxvgbpvn.html

Py:   class User: pass
来源：http://hz.ydzc1.top/gtwlucbyjc.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtvdgrhvau.html

JS:   class User {}
来源：http://hz.chenjidiqi.icu/gtwfdmkxll.html

TS:   class User { name: string = ""; }
来源：http://hz.sweek.top/gtvpktnwxd.html

Java: class User {}
来源：http://hz.shuidangran.top/gtbqyonkbb.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtudtwfwpk.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtynyobnnl.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gtmyiqqity.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtigcctosg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtlpilbtca.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtvlryujxn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtjflinsnl.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtqlvmqudx.html

Java: User(String name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtrirlmptc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tianlin.xyz/gtdqzhbtwg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtyezvbcaw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtjdzpzvow.html

[G03] 实例属性
来源：http://hz.tanke756.top/gtdzkavpih.html

Py:   self.name = "x"
来源：http://hz.jqgfzy.top/gtolccuwcg.html

PHP:  public string $name = "x";
来源：http://hz.gaohongyu789.top/gtswfolkzw.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtvvsnmrtu.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtgixihsgg.html

Java: private String name;
来源：http://hz.shanyushiyangtech.top/gtpkcjiqdw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gtvvpfzswt.html

Ruby: @name = "x"
来源：http://hz.tanke756.top/gtbvvcbugh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gtqgltwzzo.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gtmdhzanbg.html

Py:   def greet(self): return self.name
来源：http://hz.ydzc1.top/gtmuzdmwxh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtaxyqjkjg.html

JS:   greet() { return this.name; }
来源：http://hz.jqgfzy.top/gtqhgrofex.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gtpeupqzzt.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtuoimguno.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tanke756.top/gtwzcveyav.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gthfgsiglk.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gtxznxzeqv.html

[G05] 继承
来源：http://hz.meibo888.top/gtrelexhdf.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtpoazfhvo.html

PHP:  class Admin extends User {}
来源：http://hz.ybcxt.top/gtmciyjkro.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtflkoknrl.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtacohxihb.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtojbnqhkh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtmzvpwsez.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gtriubmqiq.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtxqemvcao.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtimpfwajd.html

Py:   def greet(self): return "admin"
来源：http://hz.dashuyun.cn/gtazkrqeeh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtuwticclb.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtelkzxtcc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtivltdaeg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtjiuxcats.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gttheorvce.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gthudvdzag.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtlqlogzsz.html

[G07] 调用父类方法
来源：http://hz.zhoulong.xyz/gtmudibyqv.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtfihkixei.html

PHP:  parent::greet();
来源：http://hz.hnqzz.top/gtxpkkqruc.html

JS:   super.greet();
来源：http://hz.yuanzhike.top/gtynwwvbuu.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtoaopcmvu.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gthzeaglln.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gttckmfshu.html


<!-- 参考信息 -->