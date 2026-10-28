代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xziqi.cn/gtvaerdfww.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.havefunace.top/gtuiduhsvj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtdhzgeflx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtwkndhfxt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ppjwa.cn/gtrkvcoosu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gzhubu.top/gtttrcalpi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xziqi.cn/gtifvzuczn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gtjblxsbzb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shzxlz.cn/gtklgjjcoa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yanxiufei.cn/gtntwnwges.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cheryme.top/gtgucxglhq.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtgzjzlgkq.html

TS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtujskghje.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtqariqgpz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtlyxkhvxb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenlongwang.top/gtwdekqhgp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gtfvvudlhf.html

[E11] 反转字符串
来源：http://hz.ehwqpu.com/gtiglkftqm.html

Py:   s[::-1]
来源：http://hz.xziqi.cn/gtakulbjev.html

PHP:  strrev($s);
来源：http://hz.cheryme.top/gthnatloud.html

JS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtydtimvuc.html

TS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtwlpduccc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sufxvd.cn/gtvgpnkdcu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shangyingyoupin.top/gtraytehqv.html

Ruby: s.reverse
来源：http://hz.yj20258.top/gtbgrzruix.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtiqymgouw.html

[E12] 统计某字符出现次数
来源：http://hz.andypj.xyz/gtqtzcfqqm.html

Py:   s.count("a")
来源：http://hz.hysaishi.cn/gtbhlvxybt.html

PHP:  substr_count($s, "a");
来源：http://hz.hywenlv.cn/gtqeuykvpq.html

JS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtjivhfovf.html

TS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtnarjeddd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangdashe.top/gtyrddnuwj.html

Go:   strings.Count(s, "a")
来源：http://hz.meibo888.top/gtwvvlidbq.html

Ruby: s.count("a")
来源：http://hz.nanxinkj.top/gtdelowvdc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhijiandao.cn/gtsfkhwglm.html

[E13] 逐字符遍历
来源：http://hz.jlsjyb.cn/gtkcqlkjtg.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gtcbndndpn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.andypj.xyz/gtkkwsprja.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtqugasutb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtzthfzsxg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hysaishi.cn/gtvidmjcqj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtlbdzpcuc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hongshengwenyu.top/gtjqcaddoe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guowangkeji.top/gtnkojnmax.html

[E14] URL 编码与 Base64
来源：http://hz.zdqjudy.top/gtviecndwa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.redwolf501.top/gtsljsolin.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yueranfly.top/gtnhwnagci.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.daria6918.cn/gtvkhuzfnt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.havefunace.top/gtjwvrplxo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.quarkkingdee.top/gteewnkott.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.havefunace.top/gtzggodwdo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guannengcc.top/gtbqjnxbhw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtyrqpqdls.html

[E15] HTML 转义 / 反转义
来源：http://hz.pycfn.com/gtdopcoaks.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhoulong.xyz/gtksmaijnf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jlsjyb.cn/gtgnsoecym.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aibaodan.cn/gtjzexjyez.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtbsbwcuvd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yueranfly.top/gtrhxolzvo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigfzy.top/gtunifrshj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtmrvkxiaa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gtcnvynmpr.html

[E16] 数字千分位
来源：http://hz.xuetiantiany.cn/gtnoacfkas.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtsmahdmlg.html

PHP:  number_format(1234567);
来源：http://hz.zhixingplan.top/gtocyuyrhj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtdobyphjo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtstigtzpl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtykynyiko.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangkeji.top/gtkptnhycx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xylfe.cn/gtahrikphi.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtdyivzsrp.html

[E17] 首字母大写
来源：http://hz.dianchejie.cn/gtixkzvueq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fzhhl.top/gtvumqpdlq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gtoeogszyr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtqjasxaww.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtwqcejpbj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.svipenyu.cn/gtftxbqqth.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tian-w.cn/gtpsassudh.html

Ruby: s.capitalize
来源：http://hz.yongpay.top/gtafkdokqb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shzxlz.cn/gtmylorqhq.html

[E18] 模板占位符替换
来源：http://hz.pycfn.com/gtrmgrykeg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sufxvd.cn/gtkpmsmbnu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtyrgmuird.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xinyue.icu/gtgvniahxe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtwqrntvbr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jianghu66.top/gtvnfqplwt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gtymzwjeay.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.mhx1999.top/gtjlavffbj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xziqi.cn/gtfpvsnsmg.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gtrabopnii.html

Py:   s.splitlines()
来源：http://hz.hnqzz.top/gtztkrsdsv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenlongwang.top/gtqvqhwbie.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtleznaudi.html

TS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtrygdjmac.html

Java: s.lines().toList()
来源：http://hz.sufxvd.cn/gtjjchpzfc.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtklkxtcpc.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtlyynaqck.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtwfifeomo.html

[E20] 判断字符串是否为空
来源：http://hz.xuetiantiany.cn/gtnwtwzhps.html

Py:   if not s:
来源：http://hz.cashguo.top/gtqygsscbk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhaomingkeji.xyz/gtwdfkomqj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guannengcc.top/gtoogpjwkr.html

TS:   if (s === "") {}
来源：http://hz.havefunace.top/gtovyyhyte.html

Java: if (s.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtcgtzbcnl.html

Go:   if s == "" {}
来源：http://hz.quarkkingdee.top/gtbcexgboc.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtdpjhgppy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.316326.xyz/gtiuegfukm.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtuncxlxbs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtoyqpxaxz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtditocigs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtqmsibnoo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtywbfzlua.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtikcnxsmj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenlongwang.top/gtzmxbspmp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenzaomai.com/gteeilhazi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtxtkccokc.html

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtkmcunope.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.meibo888.top/gtuecoylnj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtdwxgcuvj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gteuxxhjct.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtyexbhszi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yangfankeji.com/gtcseblfbr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhengqikj.top/gtvvqolork.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuetiantiany.cn/gtdvbzyhev.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtbyrjoxcv.html

================================================================================
来源：http://hz.sysykeji.top/gtqwlojzcg.html

F. 文件与目录
来源：http://hz.tian-w.cn/gtxzlawmql.html

================================================================================
来源：http://hz.aizwys.cn/gthzvqrmxa.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtaoidzinj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtcgakkisu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtrbbpsxkf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenlongwang.top/gtcrbzrwvx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtkqnswoaz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtuadmqdml.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgufenzy.top/gtzqbzeyvd.html

Ruby: File.read("a.txt")
来源：http://hz.zhijiandao.cn/gtqtzczyrr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zdqjudy.top/gtlzqbuqgg.html

[F02] 逐行读取文件
来源：http://hz.quarkkingdee.top/gtcqlnacfa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gtutyinyqv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtcqcbcgjn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gttjbretlv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtzegjoehf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xziqi.cn/gtjcqwxzku.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gtqcbpfxmy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shuidangran.top/gtatmcsnra.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhongyouzk.top/gttimuxzcf.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigfzy.top/gtsfijdxzf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xinyue.icu/gthjjtdbbx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtmcnfysnw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtjidnzdul.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtsvrxwdna.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gteevbezgm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yueranfly.top/gtivczgbjf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhiwuduotai.top/gthtrntxtd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtqzbetadl.html

[F04] 追加写入文件
来源：http://hz.tian-w.cn/gtbwbbjipp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhaomingkeji.xyz/gthrqtbjhv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guowangkeji.top/gtxwzoegmh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtvwjlnucw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtquokdceo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gtlbnqmdju.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtsediaqpn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtcijvjoao.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hongshengwenyu.top/gtjbstcoky.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtlxlvearb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yonumen.top/gtsdzmiljl.html

PHP:  file_exists("a.txt");
来源：http://hz.aibaodan.cn/gtmwkdazdf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtjcgxrnth.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtidcggbuh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtwwhnvqvn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.haohaochexian.top/gtsdzpempc.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenzaomai.com/gtkginwltr.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtwkfcpqyd.html

[F06] 删除文件
来源：http://hz.hnqzz.top/gtkjkvtskf.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtijdjncwf.html

PHP:  unlink("a.txt");
来源：http://hz.gzhubu.top/gtcxcovxey.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtormuizvp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtyyxzkqwu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtiunwrtvn.html

Go:   os.Remove("a.txt")
来源：http://hz.yanxiufei.cn/gtxmmvwpgd.html

Ruby: File.delete("a.txt")
来源：http://hz.wangdashe.top/gtoixauloy.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtvudzjsgk.html

[F07] 创建目录（含多级）
来源：http://hz.tanke756.top/gtkaievhlz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtyztiahsn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhixingplan.top/gtexfpgjmk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtphivondp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtvgdgjfku.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtxwyozery.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtclxruxtz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtagmglsuh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dianchejie.cn/gtthmwfhia.html

[F08] 遍历目录
来源：http://hz.cucudq.cn/gtshzscggg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pycfn.com/gtzrgbjrwm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ivvv.top/gtlxsqgwom.html

JS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtzwgboewu.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtmrtkozar.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtvtddpjht.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ehwqpu.com/gtbfkzumft.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtrwjtrnyo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.snrcjt.cn/gtungyhjup.html

[F09] 获取文件大小
来源：http://hz.sysykeji.top/gtdvrklqax.html

Py:   os.path.getsize("a.txt")
来源：http://hz.feifeiyinyue.top/gtlhctxfoa.html

PHP:  filesize("a.txt");
来源：http://hz.fengsongda.top/gtjouczwvc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtzoksynck.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtmyfrfepm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtwjgjabsr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtlyhwqnsn.html

Ruby: File.size("a.txt")
来源：http://hz.daxiang520.top/gtwhyeuvmp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhongyouzk.top/gtwdgscjiv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xziqi.cn/gtbdpnimku.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtrbktdgjz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtzmgfazja.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtwvqukqle.html

TS:   path.extname("a.txt")
来源：http://hz.hnxiangtu.top/gtzanjucye.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shangyingyoupin.top/gtgdguuabj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtbuiryprq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtwwmvlliv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtbbhnvkfp.html

[F11] 复制与移动文件
来源：http://hz.yueranfly.top/gtiqjsewhh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtrdyakvbk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sxryk.cn/gtseukorsv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtwqivngft.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtacvmfnjv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigfzy.top/gtbvwcrfzz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtgzhdespd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sweek.top/gthoemefjj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daxiang520.top/gtrqquwexj.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gtqxncncym.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuanzhike.top/gtupnccjna.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtgyvfadau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cashguo.top/gtrcufscbf.html

TS:   // 同上
来源：http://hz.hnxiangtu.top/gtpqefnbaf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cheryme.top/gtferkwpjc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.feifeiyinyue.top/gtwmjglkts.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtzaenppaj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtlsqubhqf.html

================================================================================
来源：http://hz.yuanzhike.top/gtsbyfiyuu.html

G. 面向对象
来源：http://hz.haohaochexian.top/gtesnglnwr.html

================================================================================
来源：http://hz.andypj.xyz/gtxijomdcj.html

[G01] 定义类
来源：http://hz.jinyuanbaomall.cn/gttuqdstvm.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtjamlxuru.html

PHP:  class User {}
来源：http://hz.yuxming.cn/gtyivksgqw.html

JS:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtihzzeacz.html

TS:   class User { name: string = ""; }
来源：http://hz.pengpengdd.cyou/gtvododrcu.html

Java: class User {}
来源：http://hz.fzhhl.top/gtucwendsh.html

Go:   type User struct { Name string }
来源：http://hz.dashuyun.cn/gtiejsufpc.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtetvtjgcq.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gtvsorgpqk.html

[G02] 构造函数
来源：http://hz.fengsongda.top/gtklivmsgu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ehwqpu.com/gtcvvzlbju.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxinkj.top/gtnaufheko.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtzftkhfvg.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtxwsuapqk.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtyknfaesq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xingfuxueyuan.xyz/gtxbudvkfg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtadyccovi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydzc1.top/gtpjsrsivm.html

[G03] 实例属性
来源：http://hz.yangfankeji.com/gtobaurior.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtpzneeaxl.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtznppjgoj.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtfspmeasr.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtmytzsxsw.html

Java: private String name;
来源：http://hz.zycfv.cn/gtyacwuznh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gtxwedptgt.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtozvfnnir.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtzdthyksg.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtlleipmap.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtipjjtfuo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtguexwkkc.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtotcaogri.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtonyfdeff.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtqfotxjwo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtyqrwixjm.html

Ruby: def greet; @name; end
来源：http://hz.smart0.xyz/gtaxglavan.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtxfsapmve.html

[G05] 继承
来源：http://hz.haohaochexian.top/gtnvnjhsys.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtngrqlmyy.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtbfufmpik.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtfnrtbgem.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtfcbyapwz.html

Java: class Admin extends User {}
来源：http://hz.sysykeji.top/gttzcjqjlt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.c1oappe.top/gtdkzdluxa.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gtovoqdalf.html

C#:   class Admin : User {}
来源：http://hz.wangdashe.top/gtjentncaf.html

[G06] 重写方法
来源：http://hz.redwolf501.top/gtplhqowwy.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtpkdmcjeg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtzybtcwkt.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtuuwadnqm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtgxesthks.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtqotrwhev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gtawdhajto.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtolrfakzr.html

C#:   public override string Greet() => "admin";
来源：http://hz.zycfv.cn/gtgsrgwpgs.html

[G07] 调用父类方法
来源：http://hz.hnqzz.top/gtkqmqpecq.html

Py:   super().greet()
来源：http://hz.andypj.xyz/gtqoduunye.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gtidgcrfvf.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtltwosrwv.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtfqmsnaur.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtszuyzrbt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtggjdzhwo.html


<!-- 参考信息 -->