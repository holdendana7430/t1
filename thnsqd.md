代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuanzx.com/gtrqebdvan.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gthitrgpks.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ppjwa.cn/gtexqmlcen.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtychkacnz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenlongwang.top/gtpiqqdwck.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtaynynfdp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fzhhl.top/gtsksnrzso.html

JS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtjspvqfxh.html

TS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtgnmnanzv.html

Java: String.format("%03d", 7)
来源：http://hz.guannengcc.top/gtlauvmpyu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sweek.top/gtvdlpgmta.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gtjudiemia.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gtndatvnet.html

[E11] 反转字符串
来源：http://hz.sufxvd.cn/gtdyibxvmy.html

Py:   s[::-1]
来源：http://hz.xuanzx.com/gtrsaoxnmz.html

PHP:  strrev($s);
来源：http://hz.cqqwz.cn/gtzbpirwze.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtvedkuamr.html

TS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtasdzrdlj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guowangkeji.top/gtyfvvvpgr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jianghu66.top/gtezeesing.html

Ruby: s.reverse
来源：http://hz.cqqwz.cn/gtefscqznu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtpxmogera.html

[E12] 统计某字符出现次数
来源：http://hz.sweek.top/gtnuzfisze.html

Py:   s.count("a")
来源：http://hz.ehwqpu.com/gtpodaeizk.html

PHP:  substr_count($s, "a");
来源：http://hz.shzxlz.cn/gttyopdmjn.html

JS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtzrzltnao.html

TS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtyfmithzu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.andypj.xyz/gtrwvijqky.html

Go:   strings.Count(s, "a")
来源：http://hz.ywan-chungtsiang.top/gtktbyyvbl.html

Ruby: s.count("a")
来源：http://hz.dianchejie.cn/gtpkmrzror.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nwbrower.top/gtybcqoojp.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtlbtjkfuh.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gttioiejfe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxuanxn.top/gtxzaorpjg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yongpay.top/gtvabfrpae.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtnpgmdbau.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gtcraxvfic.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtsemgcwsu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtbcoiynbq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yangfankeji.com/gtauxoblsw.html

[E14] URL 编码与 Base64
来源：http://hz.yonumen.top/gtmibmndyi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hywenlv.cn/gtmhsauubl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgufenzy.top/gtoflehmeq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dianchejie.cn/gtvsyfsrcu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ivvv.top/gtouihenlm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigufen.top/gtmcrdqauh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tianlin.xyz/gtibbyotaw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtfqlbosnx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yonumen.top/gtqmyhyymo.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtjzykvsoq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yueranfly.top/gtpvtppnhw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.bjfxy.top/gtospyxrvo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.kuanghao11.cn/gtyntcraib.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgufenzy.top/gtonrgvudg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.pycfn.com/gtwqugicsj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jianghu66.top/gtepxmpkpp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cashguo.top/gtmirlitfc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gtvrftsjys.html

[E16] 数字千分位
来源：http://hz.ehwqpu.com/gtufhzbomh.html

Py:   f"{1234567:,}"
来源：http://hz.hongshengwenyu.top/gtincwoyhs.html

PHP:  number_format(1234567);
来源：http://hz.chenzaomai.com/gtkaagneeq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtlbrjntma.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gthqptjpvm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aizwys.cn/gttibuyeag.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fzhhl.top/gtcqtsbppn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtptbhvqdw.html

C#:   1234567.ToString("N0")
来源：http://hz.yvedp.cn/gtdlxxrbfb.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtdggkybfq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtpilvjweb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtvqcgmzxr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gthpsgomuf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtxuxjmnpm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtnxtcefht.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.kuanghao11.cn/gtxampulfb.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtzljdyegz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.vqdsnc.cn/gteadwutve.html

[E18] 模板占位符替换
来源：http://hz.dashuyun.cn/gtepngjlxe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtbtecfohs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ivvv.top/gtenioodhn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtmkiuxiyr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtserehexl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gtmxmsantw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtbimnnkaf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.316326.xyz/gtqurrixwy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jlsjyb.cn/gtkkeizczy.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtptzuqdgh.html

Py:   s.splitlines()
来源：http://hz.ybcxt.top/gtzbvkaxdk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hfpthk.cn/gtrotmnpxj.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtjnnkkhhs.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtbhslqkas.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtogsxpfxh.html

Go:   strings.Split(s, "\n")
来源：http://hz.mhx1999.top/gtocriemky.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtavzhsxqr.html

C#:   s.Split('\n')
来源：http://hz.nanxuanxn.top/gtecbwtbwb.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gttgjptjhr.html

Py:   if not s:
来源：http://hz.wangdashe.top/gtxptilqef.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gtkrtchfrs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxuanxn.top/gtvdrtltaz.html

TS:   if (s === "") {}
来源：http://hz.quarkkingdee.top/gtwxogqdsz.html

Java: if (s.isEmpty()) {}
来源：http://hz.meibo888.top/gtshbrsigg.html

Go:   if s == "" {}
来源：http://hz.daria6918.cn/gtcpqdsypo.html

Ruby: if s.empty?
来源：http://hz.ivvv.top/gtmnsrwpob.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guowangkeji.top/gttrglkxxf.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gttnerrqlz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.0kj1m.cn/gtggnznfbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgfzy.top/gtkgcwzjeo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtxavlbgpj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtusyyhqfj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtauyuxbmh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gaohongyu789.top/gtpzrcduha.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yangfankeji.com/gtepdjbohp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cucudq.cn/gtzbhcfdpq.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtwkbmirtb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhixingplan.top/gtxsnahgrb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtvchhasfj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtpbrjeths.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtoxezgexa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gtzdwvukiv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gteyonehuy.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtnzcyhcim.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxinkj.top/gtzrhwvwiu.html

================================================================================
来源：http://hz.zhixingplan.top/gtgmvocchz.html

F. 文件与目录
来源：http://hz.guowangkeji.top/gtrpemkgyx.html

================================================================================
来源：http://hz.fengsongda.top/gtarbbwcgu.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtnkydofls.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigfzy.top/gtnqedahyq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigfzy.top/gtmzozpahh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtahgirhqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.redwolf501.top/gttqstmeqj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtklqljcin.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtubheohms.html

Ruby: File.read("a.txt")
来源：http://hz.haohaochexian.top/gtczahiazj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinyuanbaomall.cn/gthhesttao.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtfvyzuqgs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ybcxt.top/gtgawltanh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yongpay.top/gtpcasaaqc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtwoplyuvu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtlozbqitx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sweek.top/gtacuhvnkr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangtech.top/gtlquykxnc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtapguzpkl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.meibo888.top/gtrmatwooi.html

[F03] 写入文件（覆盖）
来源：http://hz.0kj1m.cn/gtazidnigl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ehwqpu.com/gtbsqjvxxw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtkcmmkstp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtcmdlyfku.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtsdmrbsog.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtmmnqiwdy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtqqlfkbhc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pengpengdd.cyou/gtxrogpcuo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guannengcc.top/gteolegeha.html

[F04] 追加写入文件
来源：http://hz.yueranfly.top/gtytcttvkw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgfzy.top/gtptkeresn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yanxiufei.cn/gtzpskhcae.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtdcjzxugd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtiicnxfix.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258.top/gtzsiwhfah.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtrxyohkhv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtrjapsjgz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.smart0.xyz/gtqndupkat.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxinkj.top/gtplokfjgq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtvcnjiyma.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtkjvqtgnx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtdmgugent.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtyhxtsgzs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtwqfgvcom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gtxsnehnij.html

Ruby: File.exist?("a.txt")
来源：http://hz.snrcjt.cn/gtyolytwyg.html

C#:   File.Exists("a.txt")
来源：http://hz.gaohongyu789.top/gtmsfbiudi.html

[F06] 删除文件
来源：http://hz.cucudq.cn/gtzswhjsin.html

Py:   os.remove("a.txt")
来源：http://hz.aizwys.cn/gtqxxbykab.html

PHP:  unlink("a.txt");
来源：http://hz.jlsjyb.cn/gtissybujn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gtflaqhzey.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtitfhzkqa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtoscbouxx.html

Go:   os.Remove("a.txt")
来源：http://hz.andypj.xyz/gthtctveoy.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtwipwlyrd.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gthjiiyhnx.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtaktdlzhd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxuanxn.top/gtaolzvbom.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhoulong.xyz/gtvmlsoojn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtrlajdinv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtesgmetai.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shzxlz.cn/gteohibfer.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jiagoushi.top/gtplswwsvf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gtjknwhtfp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxuanxn.top/gttttjjtci.html

[F08] 遍历目录
来源：http://hz.jqgfzy.top/gttdhpaxdw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zdqjudy.top/gtuepedijw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.0kj1m.cn/gtxrfrursm.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtatagelak.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtguiadjgf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtbtnxgspo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.vqdsnc.cn/gtwnbfusof.html

Ruby: Dir.children("dir")
来源：http://hz.quarkkingdee.top/gtujmgaufq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtcutxpxvp.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtpjurpoly.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgfzy.top/gtqdeqqqof.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtkdlttofr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtszplqxxc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtvjkihyhl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtlpxdlfje.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenlongwang.top/gtuuxbymhs.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gtxnjnbnzr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dianchejie.cn/gtweberipx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtrgfiuuhg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtmiqhqtrl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258888.top/gtnuiqcovc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtqcpxdlea.html

TS:   path.extname("a.txt")
来源：http://hz.gogol.net.cn/gtjymqpphg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yueranfly.top/gtqqzjzfwp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtfemdnbqo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtruhzxwsk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zdqjudy.top/gtjditaspj.html

[F11] 复制与移动文件
来源：http://hz.wangshuangyany.cn/gtsvnojdhx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtcogsiyoy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinyuanbaomall.cn/gtzzstklhi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtyocuovpi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtesgounji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.kuanghao11.cn/gtroukksjw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtwujmyjyq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtxxjfssyg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daria6918.cn/gtesxlzmxq.html

[F12] CSV 读写
来源：http://hz.316326.xyz/gtuzizttqu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xinyue.icu/gtbnsmfqdl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtmhdydump.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtsnxjqiih.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtwiqnvxed.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gttrtpuziz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtzqogjckr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtzalqrfal.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gtjevczbfd.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnnpipvgj.html

G. 面向对象
来源：http://hz.zycfv.cn/gtvcguhbat.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrzwmoilh.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtkewyunjl.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtslfydodp.html

PHP:  class User {}
来源：http://hz.yuxming.cn/gtshsnwxco.html

JS:   class User {}
来源：http://hz.ehwqpu.com/gtykfvofmd.html

TS:   class User { name: string = ""; }
来源：http://hz.zhiwuduotai.top/gtyxwnfpgn.html

Java: class User {}
来源：http://hz.gzhubu.top/gtggeukyde.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gttjyiawiq.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gttqnsteva.html

C#:   class User {}
来源：http://hz.xziqi.cn/gtjbnqvpbm.html

[G02] 构造函数
来源：http://hz.tanke756.top/gttplknmxs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yueranfly.top/gtloztvkjj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tanke756.top/gtaofbttro.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtshckxgkm.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gthjqklmsr.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtltmxwude.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtfweucqqv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtpmkfobcu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fengsongda.top/gtfaopwyqk.html

[G03] 实例属性
来源：http://hz.jianghu66.top/gtakkavjtz.html

Py:   self.name = "x"
来源：http://hz.feifeiyinyue.top/gtkdxkfqot.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gttvpvnjpw.html

JS:   this.name = "x";
来源：http://hz.yuanzhike.top/gthbetclbu.html

TS:   name: string = "x";
来源：http://hz.jqgfzy.top/gteoyjqrtp.html

Java: private String name;
来源：http://hz.bjfxy.top/gtqyoukkyz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yueranfly.top/gtjgwwblbe.html

Ruby: @name = "x"
来源：http://hz.tianlin.xyz/gtdyvvpvyj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.redwolf501.top/gthftcbizg.html

[G04] 定义方法
来源：http://hz.sxryk.cn/gtcrhqhxly.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtyagwhspd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtgxlkrvzx.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtsmdcwcsj.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gttuqswzxf.html

Java: String greet() { return name; }
来源：http://hz.svipenyu.cn/gtzaaennyy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cqqwz.cn/gtwvyacwes.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtrpluiwfj.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtmgarafyz.html

[G05] 继承
来源：http://hz.wangdashe.top/gtbniypiqu.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtdbwkyxoc.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtckemsfqr.html

JS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtykqaswze.html

TS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtqahisuko.html

Java: class Admin extends User {}
来源：http://hz.sysykeji.top/gtsxhvksrp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cqqwz.cn/gtjczctenu.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtijhrrnkf.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gtvqtulgek.html

[G06] 重写方法
来源：http://hz.quarkkingdee.top/gtlarsjyya.html

Py:   def greet(self): return "admin"
来源：http://hz.dashuyun.cn/gtluwnxzmk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtbyrhgqnn.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gttkawwsxb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtbkzvcodg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtmwucyffo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhijiandao.cn/gthwqjptjq.html

Ruby: def greet; "admin"; end
来源：http://hz.jlsjyb.cn/gtbucglihn.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtzydrsrxh.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gtkpnbfcqe.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtvhfvswve.html

PHP:  parent::greet();
来源：http://hz.nwbrower.top/gtjewehxtu.html

JS:   super.greet();
来源：http://hz.zhixingplan.top/gtsqenfvjl.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtmxdurbzf.html

Java: super.greet();
来源：http://hz.wangdashe.top/gtzmbknepm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhongyouzk.top/gthcxinqbt.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtokgwbmsf.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtjnuwygvg.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtceohvrka.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtdolmsoom.html


<!-- 参考信息 -->