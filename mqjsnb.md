代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.yuanzhike.top/gtqodqoxqk.html

JS:   items.join(",")
来源：http://hz.sysykeji.top/gtuwpdmgde.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtlljwvhfg.html

Java: String.join(",", items)
来源：http://hz.sufxvd.cn/gtaubzbiqq.html

Go:   strings.Join(items, ",")
来源：http://hz.yongpay.top/gtqchgyrkr.html

Ruby: items.join(",")
来源：http://hz.yvedp.cn/gtrsxhsptj.html

C#:   string.Join(",", items)
来源：http://hz.ehwqpu.com/gtvcxsihdm.html

[E09] 去除所有空白字符
来源：http://hz.hywenlv.cn/gthzbfqanx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gtbppjomaq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.fzhhl.top/gtfanfpova.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtgpnvhquw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gthxiircuj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.vqdsnc.cn/gtkhucbwso.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dianchejie.cn/gtagxljzte.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gteuuxrdfc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nanxuanxn.top/gtxlcupmcu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.havefunace.top/gtllpjbzov.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj20258.top/gtiaokamop.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtbtbahxlj.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtlvutrohh.html

TS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtlcchvsst.html

Java: String.format("%03d", 7)
来源：http://hz.mhx1999.top/gtgubthsbu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.birdmap.top/gtdtrvmhgu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtricvszls.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtlisanonl.html

[E11] 反转字符串
来源：http://hz.gzhubu.top/gtawrsdyou.html

Py:   s[::-1]
来源：http://hz.ivvv.top/gtqdvbzrnf.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gtulrafbhy.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtpvuwzhhu.html

TS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtaenuvibm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtwiovxxqg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shuidangran.top/gttzclsmfp.html

Ruby: s.reverse
来源：http://hz.dashuyun.cn/gtodzruszn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gthnjxxzro.html

[E12] 统计某字符出现次数
来源：http://hz.jianghu66.top/gtpjxzclak.html

Py:   s.count("a")
来源：http://hz.ybcxt.top/gtcucjyblg.html

PHP:  substr_count($s, "a");
来源：http://hz.c1oappe.top/gthbaxvatg.html

JS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gtpdzjhklz.html

TS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtmsrxlmbe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtiouqbyku.html

Go:   strings.Count(s, "a")
来源：http://hz.xingfuxueyuan.xyz/gtcjgtkcwl.html

Ruby: s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtulxjqmlq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtejglzbqu.html

[E13] 逐字符遍历
来源：http://hz.hnxiangtu.top/gtzuweaqot.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gtxnluevzx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jianghu66.top/gtrkqnblan.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtbiwiwnbb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtipzozzvt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhixingplan.top/gtifjzcpwb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.316326.xyz/gthyftjbii.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtleibokhx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtyusclcdj.html

[E14] URL 编码与 Base64
来源：http://hz.zhongyouzk.top/gtsumgfgka.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.andypj.xyz/gtuhsoyegp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.andypj.xyz/gtcvnsrbsy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shangyingyoupin.top/gtihcjxgen.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenlongwang.top/gtzxvesqtd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sufxvd.cn/gtiopqwozt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ehwqpu.com/gttumsqgoa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.vqdsnc.cn/gtvlypynde.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jyoumei.cn/gtmjtugylw.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinghuilouyu.cn/gtssoewcdm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ppjwa.cn/gticutgvpm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yvedp.cn/gtoogbrsia.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtibrgeptr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tanke756.top/gtptjkkeqd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.quarkkingdee.top/gtzigrfmkf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenjidiqi.icu/gtkeuixrox.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtlmulskso.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtbydyylks.html

[E16] 数字千分位
来源：http://hz.guannengcc.top/gttqjnwquy.html

Py:   f"{1234567:,}"
来源：http://hz.chenjidiqi.icu/gtjsyovjlw.html

PHP:  number_format(1234567);
来源：http://hz.zhaomingkeji.xyz/gtpqxtxabd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtwllbusiw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtvfvdqsca.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hysaishi.cn/gtpyqnsrcm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinyuanbaomall.cn/gtrgyxsxhp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydzc1.top/gtvaameems.html

C#:   1234567.ToString("N0")
来源：http://hz.aizwys.cn/gtjgrhexay.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtbiksaptt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258.top/gtudxbkakp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtgheuyzxr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtmkmavozi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.meibo888.top/gtkcohsqip.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.haohaochexian.top/gtgqtboaei.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.svipenyu.cn/gtndbnjhrn.html

Ruby: s.capitalize
来源：http://hz.hywenlv.cn/gttouanlgv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aizwys.cn/gtigmjwdur.html

[E18] 模板占位符替换
来源：http://hz.316326.xyz/gtdwfwxsfk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangtech.top/gtmctszzic.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtscuziyzm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtiqclcnne.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gteatvzzij.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtawlhjlpu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cqqwz.cn/gtsllsvsmn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtpniafwaw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtpkpftzsq.html

[E19] 多行文本按行拆分
来源：http://hz.birdmap.top/gtvkabequo.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtqrxvcwvj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtmbdpmkwc.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gthqrzxuuj.html

TS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gtzfpmnanq.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtpofljmxq.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydjk.org.cn/gtteffgwjt.html

Ruby: s.lines
来源：http://hz.gotoacloud.top/gtkroyfqme.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gtfnzdebnw.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtpjynlipq.html

Py:   if not s:
来源：http://hz.cheryme.top/gtcycrwxuz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtwedqtulf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gotoacloud.top/gtnzamgzkl.html

TS:   if (s === "") {}
来源：http://hz.hongshengwenyu.top/gtqyhgjmct.html

Java: if (s.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtlftbnbqg.html

Go:   if s == "" {}
来源：http://hz.zhaomingkeji.xyz/gtvjaehocg.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtogoxkudc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xylfe.cn/gtkflpbvfv.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtbnndjjfg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhixingplan.top/gttuytmsin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ydjk.org.cn/gtjbceecpb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtpskzcqdv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtmakripkv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtnvwdnnwa.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jyoumei.cn/gtyycwalcn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenzaomai.com/gtybeuhsny.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtaiwzjrmn.html

[E22] 字节长度与字符长度
来源：http://hz.cashguo.top/gtlfdtppwj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hammf.cn/gtoddrzfks.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtmofdexgh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtzpmirnwq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtzdwwefvx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gteelynvqn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gteteamsou.html

Ruby: s.bytesize;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtcvknhbyz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.vqdsnc.cn/gtpiorvufq.html

================================================================================
来源：http://hz.ybcxt.top/gtwqnachho.html

F. 文件与目录
来源：http://hz.yonumen.top/gtlossnvkv.html

================================================================================
来源：http://hz.iojbl.cn/gtjodpesxk.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtlvqsszru.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtlhnzcqpf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtqhblehbp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtwolposyu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtimtbjwgx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtkpxiwuuv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtkijlsrdp.html

Ruby: File.read("a.txt")
来源：http://hz.jinghuilouyu.cn/gtzstbuehk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gtewhhbemw.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtmvybbbhh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dashuyun.cn/gtpxpmplrq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sxryk.cn/gtvhjzeumk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtwwdzwmyw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtwibfveka.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtsmwjwrur.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtdqezkznd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangdashe.top/gtuhreihga.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtbhiqzmxe.html

[F03] 写入文件（覆盖）
来源：http://hz.bjfxy.top/gtdilnmmix.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xinyue.icu/gtxlximgts.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtkxkrkexk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtmxgcbqys.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtwlnsnwlr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.9152youxi.cn/gtsodafovj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258888.top/gtyohkctws.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuanzx.com/gtxxococop.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.andypj.xyz/gtiuqtgnfe.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtsondrnhi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtlgbykjqc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhoulong.xyz/gtappqndtw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtotwwfzaj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtcdlqnegs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxuanxn.top/gtvgujovja.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sysykeji.top/gtqbagwyzl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shanyushiyangtech.top/gtczdtoyrf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ppjwa.cn/gtaleeinqu.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnxiangtu.top/gtcuoccmnz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhixingplan.top/gtqqgwttaj.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtdleyjimb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtkqkrzfdr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtinpyupgu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtswuzygtp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.svipenyu.cn/gtlpvwevav.html

Ruby: File.exist?("a.txt")
来源：http://hz.jiagoushi.top/gthhvxffjh.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gtyqlwhkug.html

[F06] 删除文件
来源：http://hz.9152youxi.cn/gtxaqguupm.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtlklfberr.html

PHP:  unlink("a.txt");
来源：http://hz.tianlin.xyz/gtwphjqter.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtulicnvti.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtghqajkgz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtjorbwffv.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtjlpipsxt.html

Ruby: File.delete("a.txt")
来源：http://hz.quarkkingdee.top/gthcszbwkg.html

C#:   File.Delete("a.txt");
来源：http://hz.shangyingyoupin.top/gtyqfrfkfr.html

[F07] 创建目录（含多级）
来源：http://hz.meibo888.top/gtvwcosxmq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dianchejie.cn/gthbkvpjns.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydzc1.top/gtvucmybps.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtpzmqstnz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtmpkfmvrv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jlsjyb.cn/gtxxgzhxtu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.snrcjt.cn/gtznawujmy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hysaishi.cn/gtecbgpdvm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tanke756.top/gtxhcrssdf.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtpwgsgzdd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aibaodan.cn/gtsmqlaofo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtvncgnfsd.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtmiollzga.html

TS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gthzvyyatm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtlprjvnnk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtcsknmbxe.html

Ruby: Dir.children("dir")
来源：http://hz.jqgufenzy.top/gtxvaargbj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.bjfxy.top/gtnbpkqlue.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtplhvnhso.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gttjjycfjr.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtgewdplwq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtmeqkbxyh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gotoacloud.top/gtnwxkgevj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtckkklxsa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtlbjuiisw.html

Ruby: File.size("a.txt")
来源：http://hz.jinyuanbaomall.cn/gteummdyex.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tanke756.top/gtilnajpqr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangshuangyany.cn/gtnknryzlm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtoegxklps.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jyoumei.cn/gtmdpxjcyt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtrojimmed.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtthinwzht.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtddhfaduj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cucudq.cn/gtkmwxbbtk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtkdwgsnue.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hammf.cn/gtdxrgkska.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtfuyulran.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtnmzvlzxm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gthdinvrvm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtgsgrhphd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtvezpzjex.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtvgohjvvn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtuszzrgyt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtiwztvgss.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sufxvd.cn/gtemfpsuss.html

[F12] CSV 读写
来源：http://hz.chenlongwang.top/gtcdvrsgxh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ywan-chungtsiang.top/gtbnjjablh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydjk.org.cn/gtyjbcwrvc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtspwbcjbe.html

TS:   // 同上
来源：http://hz.havefunace.top/gtssagsanf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.smart0.xyz/gtoyhhvrgf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pycfn.com/gtmnvuqess.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zdqjudy.top/gtqvjmtpzl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.haohaochexian.top/gtfxcleyle.html

================================================================================
来源：http://hz.gogol.net.cn/gtznpjoggx.html

G. 面向对象
来源：http://hz.yonumen.top/gtqwhrdpvt.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxnsvfqjm.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtqifkewzg.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gtfgtijrzt.html

PHP:  class User {}
来源：http://hz.ivvv.top/gtikkdhkqv.html

JS:   class User {}
来源：http://hz.pycfn.com/gtstcoktjm.html

TS:   class User { name: string = ""; }
来源：http://hz.ybcxt.top/gtfxtmmlji.html

Java: class User {}
来源：http://hz.tian-w.cn/gthgfvdgnp.html

Go:   type User struct { Name string }
来源：http://hz.ybcxt.top/gtnnguikeh.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtcalkmbih.html

C#:   class User {}
来源：http://hz.yj20258888.top/gtdcwwfses.html

[G02] 构造函数
来源：http://hz.pycfn.com/gtlhuxjjyd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtogijaxjk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dashuyun.cn/gtotsyrdyr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.c1oappe.top/gtdmnqagkc.html

TS:   constructor(public name: string) {}
来源：http://hz.ydzc1.top/gtboqwwcoo.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtaxramfii.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtakfrkzdm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.smart0.xyz/gtscaxtbdd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yanxiufei.cn/gtvsyivasy.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtqduqvffs.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtiqblmrcr.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtjoedzjqd.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gtjinzvqap.html

TS:   name: string = "x";
来源：http://hz.ydzc1.top/gtnxsyzrsr.html

Java: private String name;
来源：http://hz.chenzaomai.com/gtnybznrdk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangdashe.top/gtgkjpwice.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gtnbqpiczn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtmregqwbo.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtwgkbwjoj.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gteawokekf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtqimhmmzj.html

JS:   greet() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtaxkvsrvf.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gttfnmtfrl.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtldwytytm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtoprkuoyr.html

Ruby: def greet; @name; end
来源：http://hz.hnqzz.top/gtfntzsutv.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtfxjhamjf.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtbddxlurw.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtxpxiyctw.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gturizbwtu.html

JS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtsphmxnuo.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtjdkvywht.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtzpubfxbl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ehwqpu.com/gtvzcftvxq.html

Ruby: class Admin < User; end
来源：http://hz.dashuyun.cn/gtwteakrmg.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtorlyuina.html

[G06] 重写方法
来源：http://hz.nanxuanxn.top/gtlxpzzuhy.html

Py:   def greet(self): return "admin"
来源：http://hz.bjfxy.top/gtvbxupnta.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtfoqqwolm.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtcvldlfre.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtfhfshhck.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtxfazptvc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtvtenuyid.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtjrzutham.html


<!-- 参考信息 -->