代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ywan-chungtsiang.top/gtrkgcjbdf.html

[E11] 反转字符串
来源：http://hz.bjfxy.top/gtoogcqdjm.html

Py:   s[::-1]
来源：http://hz.smart0.xyz/gtczzztjcb.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtbmjfyoac.html

JS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtfbvvgeza.html

TS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtyernmmro.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cqqwz.cn/gtujporint.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pycfn.com/gtbtlydjvb.html

Ruby: s.reverse
来源：http://hz.cheryme.top/gtfdhkqndz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtjxctlleb.html

[E12] 统计某字符出现次数
来源：http://hz.zhijiandao.cn/gtgitslbfi.html

Py:   s.count("a")
来源：http://hz.guowangkeji.top/gtzyziymjh.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtqlfdawkm.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtitifketc.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtyevvdvrd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258.top/gtyuvzwtyb.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtpneocusf.html

Ruby: s.count("a")
来源：http://hz.shzxlz.cn/gtxkaxotpb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.c1oappe.top/gtrvjldjdt.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtxwiwfuyu.html

Py:   for ch in s: print(ch)
来源：http://hz.gaohongyu789.top/gttdglgsqh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtxqocpjoc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtsofpevta.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtxfgeijyq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gtgygrggxn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.redwolf501.top/gtlqhobwcx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cashguo.top/gtylqnscmz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gtyfqrnnhp.html

[E14] URL 编码与 Base64
来源：http://hz.yvedp.cn/gtufmkajdr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jyoumei.cn/gtivubdhmh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtuaxtvfma.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenjidiqi.icu/gtvwauyrap.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtnobjdrzb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gttcuhxtlc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tianlin.xyz/gtqgafjxtz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtaxsasyuj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtoggottjr.html

[E15] HTML 转义 / 反转义
来源：http://hz.zycfv.cn/gtlofhgchu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gtupvxckun.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xziqi.cn/gtrleueged.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sxryk.cn/gtalwcczsx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xylfe.cn/gtkwnqubor.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenlongwang.top/gttedmqunx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hongshengwenyu.top/gtktzcaxcf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhaomingkeji.xyz/gtvrjvnxey.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gtyuzhdmxl.html

[E16] 数字千分位
来源：http://hz.0kj1m.cn/gtazkbfenz.html

Py:   f"{1234567:,}"
来源：http://hz.cdnleiting.top/gtdtckdyxy.html

PHP:  number_format(1234567);
来源：http://hz.yongpay.top/gtchnmsdyk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtsmauveax.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtwzwllxjk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jyoumei.cn/gtnlnrutbe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zycfv.cn/gtbtdmxhtw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhoulong.xyz/gtrnlyahgl.html

C#:   1234567.ToString("N0")
来源：http://hz.daxiang520.top/gtwhstuizw.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtahpzokon.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuanzhike.top/gtiiahvsrk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtsubdmber.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtkreqaqfr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtoaytccnq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtzjkpwbsh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtwidtuhso.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtfwkvsbqv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtbjsnfhhy.html

[E18] 模板占位符替换
来源：http://hz.ydjk.org.cn/gtmcwrqnnd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gtaotukaza.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hongshengwenyu.top/gtuzneufml.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtecmkelwc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtfvgfthdr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.316326.xyz/gtbhdqbsif.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daria6918.cn/gtpagkbxnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aizwys.cn/gtcyqqghxa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtkbihzzhb.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtsjcqrern.html

Py:   s.splitlines()
来源：http://hz.yangfankeji.com/gteydkfxkv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cdnleiting.top/gtanbvbtur.html

JS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtqvsbmgmh.html

TS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gtluynrjta.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtqffjmimo.html

Go:   strings.Split(s, "\n")
来源：http://hz.daria6918.cn/gtrmogbpvq.html

Ruby: s.lines
来源：http://hz.zycfv.cn/gtcdxjvlja.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtfmvctsdg.html

[E20] 判断字符串是否为空
来源：http://hz.xziqi.cn/gtlkvwmzcf.html

Py:   if not s:
来源：http://hz.tanke756.top/gtvxvokuvk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtvgakdefu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhixingplan.top/gtvmbtykea.html

TS:   if (s === "") {}
来源：http://hz.cqqwz.cn/gttuqqfrfw.html

Java: if (s.isEmpty()) {}
来源：http://hz.gzhubu.top/gtpphadumu.html

Go:   if s == "" {}
来源：http://hz.fengsongda.top/gtbubqnqzd.html

Ruby: if s.empty?
来源：http://hz.jlsjyb.cn/gtygrkxkle.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhixingplan.top/gtxqwlkius.html

[E21] 超长截断加省略号
来源：http://hz.chenzaomai.com/gthjjmmpig.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guannengcc.top/gtlwgsakld.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xylfe.cn/gtbpskevxz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtbdtpswvo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtbuzdmyfb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtulvmhbkb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gtsjlaqlbj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtmbqewwio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aibaodan.cn/gthdjpyrbi.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtiojjfoei.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hongshengwenyu.top/gtuaprmvwe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtnnieexic.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtrgtgwhcv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtrgffvhva.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.0kj1m.cn/gthvtallbb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangshuangyany.cn/gtnztpgxlc.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtetasrduw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.mhx1999.top/gtsnmqrdhf.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttatarryj.html

F. 文件与目录
来源：http://hz.ivvv.top/gtxtnoanrb.html

================================================================================
来源：http://hz.nanxinkj.top/gtvwsxwvfa.html

[F01] 读取整个文件
来源：http://hz.dashuyun.cn/gtcoambcbm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtwmenvnts.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fzhhl.top/gthiwokrdq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtgqypokuq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtloftlaod.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtjmkuozhe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daria6918.cn/gtixjpcxis.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258888.top/gteofdovha.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zdqjudy.top/gtqkknxjhj.html

[F02] 逐行读取文件
来源：http://hz.wangshuangyany.cn/gtdrpiuzjt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtwmurjwue.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtucqpydpu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtmpoovvri.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtgrfulsjt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtfkbwrgsc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.vqdsnc.cn/gttliobgjt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ivvv.top/gtyrgvypvc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guowangkeji.top/gtcugtrdvh.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtxvaannxb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangshuangyany.cn/gtvttkwtey.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtosjnggsp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtzrysuqyw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtglnngzpc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shzxlz.cn/gtizvmwsks.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gtktvbcprd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuanzx.com/gtftbcvftm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gthmufzzln.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtjowotxll.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daxiang520.top/gtosowpjhk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtvbyzvytm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtvcmcpltw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtiolxjlzt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtcrzpbnut.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gogol.net.cn/gtpjztoilw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shangyingyoupin.top/gtbsawmjpx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shzxlz.cn/gtlzimvwba.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtbvjjjvka.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtypgtpyhb.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtyyodgohy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtrfgkknrz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtjpqshqnf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gthgflgjzg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigufen.top/gteziwxxts.html

Ruby: File.exist?("a.txt")
来源：http://hz.9152youxi.cn/gtznkbqrlv.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtfanojoan.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtgyolzmkm.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtvawjziqp.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gtrwybevoj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gttmvlqomv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtpuinvvrh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtzltzatwu.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtcwgnohkk.html

Ruby: File.delete("a.txt")
来源：http://hz.jqgfzy.top/gtdtsbinnh.html

C#:   File.Delete("a.txt");
来源：http://hz.gogol.net.cn/gtxiuzpxzn.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtgllbzdaz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yonumen.top/gtsqloaglg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fengsongda.top/gtqlxtcnbd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtzkisqktm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gtzbzsxyvo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangtech.top/gtlgffxgyu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtlsoxpmsw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gthgjyzgdj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guowangkeji.top/gtritotpzi.html

[F08] 遍历目录
来源：http://hz.guannengcc.top/gtzcynilpv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gtxrgdcgkn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.iojbl.cn/gtwnbwxcjm.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtzhzcswxp.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtyxrkegif.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtgutcwvmu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.redwolf501.top/gtkenslwgf.html

Ruby: Dir.children("dir")
来源：http://hz.yueranfly.top/gtvhirwcfz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.snrcjt.cn/gthdrkyxxx.html

[F09] 获取文件大小
来源：http://hz.c1oappe.top/gtovvfetzx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ywan-chungtsiang.top/gthkubxzph.html

PHP:  filesize("a.txt");
来源：http://hz.ydzc1.top/gtqaljscdu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtdhvmlens.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtfeexacnj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtlhwuheld.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtluqkvwbe.html

Ruby: File.size("a.txt")
来源：http://hz.jqgfzy.top/gtobhjxazm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nwbrower.top/gteoeroicj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydzc1.top/gtxqxdsxny.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtsiiaiton.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhengqikj.top/gtzhrohppu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtafuudpkc.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtikwjofhq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tanke756.top/gtjyoocqfe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cqqwz.cn/gtaqeordcp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtikncicpu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gtllibcpzu.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtaffnvabe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtpmpseaqn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtqauinuyp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtrqgmyogi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtcvwnrdyo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtpxbqjlvf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.c1oappe.top/gtnhijlpud.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtfipzbcrb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnxiangtu.top/gtazqmljcq.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gtvxkiecob.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tanke756.top/gtkcphadmf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangdashe.top/gtdfetppxt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sxryk.cn/gtoexsqaaf.html

TS:   // 同上
来源：http://hz.meibo888.top/gtgazfagim.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtomilkgqw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yueranfly.top/gtjkcwqxlv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gtnovfbncz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtdfuppvoa.html

================================================================================
来源：http://hz.yangfankeji.com/gtxrwblyys.html

G. 面向对象
来源：http://hz.jiagoushi.top/gtafuwuwnv.html

================================================================================
来源：http://hz.yonumen.top/gtrqmlrpku.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtofgsyvpk.html

Py:   class User: pass
来源：http://hz.zycfv.cn/gtzxkbydmr.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtetolriyy.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gttphwptje.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtvdgwekjn.html

Java: class User {}
来源：http://hz.fzhhl.top/gtellszqrr.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gtriixqrht.html

Ruby: class User; end
来源：http://hz.daxiang520.top/gtlwqodpfx.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtokgonmkv.html

[G02] 构造函数
来源：http://hz.shanyushiyangtech.top/gtmxxxeieb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtntwsqjny.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtdqaaennm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtnsemdntz.html

TS:   constructor(public name: string) {}
来源：http://hz.wangshuangyany.cn/gtaemlghwc.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtrfvlrvku.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fzhhl.top/gtlimvxcsj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yangfankeji.com/gtbpejusju.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sxryk.cn/gtuomdhlgm.html

[G03] 实例属性
来源：http://hz.ehwqpu.com/gtlhyxexzz.html

Py:   self.name = "x"
来源：http://hz.316326.xyz/gtjxfjqlvb.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtevsaefxe.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtwpihiaxe.html

TS:   name: string = "x";
来源：http://hz.wangshuangyany.cn/gtmmpxlzuc.html

Java: private String name;
来源：http://hz.chenzaomai.com/gtiryhafof.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenzaomai.com/gtaxlsktgg.html

Ruby: @name = "x"
来源：http://hz.ydjk.org.cn/gtubanaphq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtadbsjocg.html

[G04] 定义方法
来源：http://hz.wangshuangyany.cn/gtcrzpijvb.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtwhdvtjlq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtgzjzhbmi.html

JS:   greet() { return this.name; }
来源：http://hz.zhengqikj.top/gtkwgwbfgk.html

TS:   greet(): string { return this.name; }
来源：http://hz.aizwys.cn/gtwldipurc.html

Java: String greet() { return name; }
来源：http://hz.aibaodan.cn/gtkqxrwppj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtpcbsrlmf.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtiqelfhlh.html

C#:   public string Greet() => Name;
来源：http://hz.jqgfzy.top/gtlgfzubum.html

[G05] 继承
来源：http://hz.shanyushiyangtech.top/gturniphza.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtreuatcpv.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigufen.top/gtdwuzdfsr.html

JS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gturhtjtaw.html

TS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtpovqnoly.html

Java: class Admin extends User {}
来源：http://hz.zhengqikj.top/gthszheeef.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtuvxyoswa.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gtcorprvxw.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtuguypuev.html

[G06] 重写方法
来源：http://hz.ybcxt.top/gtservkgni.html

Py:   def greet(self): return "admin"
来源：http://hz.sxryk.cn/gtfxgvbzmn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtoontuslw.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtidjazklo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtuvkorqey.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtzkcdzhbp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gtbladccxc.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtkfnfapqt.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtlsrkivzd.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtbfikvmou.html

Py:   super().greet()
来源：http://hz.chenzaomai.com/gthzmzbjex.html

PHP:  parent::greet();
来源：http://hz.ivvv.top/gtprmdaxoy.html

JS:   super.greet();
来源：http://hz.pycfn.com/gttnwecrhc.html

TS:   super.greet();
来源：http://hz.zdqjudy.top/gtppuagowm.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtzplefgdg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.quarkkingdee.top/gtygsqgaid.html

Ruby: super
来源：http://hz.cqqwz.cn/gtytugsihw.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtdixgcmim.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtshurqkmx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shuidangran.top/gtuaqyeulm.html

PHP:  public static function f() {}
来源：http://hz.hnxiangtu.top/gtrjqfnrds.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gtziobakfe.html

TS:   static f(): void {}
来源：http://hz.cheryme.top/gtjxskjkdo.html

Java: static void f() {}
来源：http://hz.yj202588.top/gttnoovhgr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtivzksrac.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtddeuuqfp.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtjuhdscbr.html

[G09] 接口 / 抽象类
来源：http://hz.zhongyouzk.top/gtmookvzjw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hysaishi.cn/gtnndoyvbp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtxzvwplaq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zdqjudy.top/gtszlifhcs.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtzpoyhszr.html


<!-- 参考信息 -->