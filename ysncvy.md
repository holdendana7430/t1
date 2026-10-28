代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gtocpboyxf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xinyue.icu/gtgnbmnsne.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtzoxsczdb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtqlrkmjfy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhiwuduotai.top/gtofrzjkrh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cqqwz.cn/gtykhdeuwx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gtcevnsvje.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.52xcode.cn/gtsajwjmps.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hammf.cn/gtxuxyqsst.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnqzz.top/gteelprtnq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.0kj1m.cn/gtlskkeelr.html

JS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtgkcdipaj.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtxllizppz.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gtlvyyjogt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ehwqpu.com/gtqrrmmmmy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dianchejie.cn/gtygqeswdy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.smart0.xyz/gtuufjwuzl.html

[E11] 反转字符串
来源：http://hz.smart0.xyz/gtpfcixgzu.html

Py:   s[::-1]
来源：http://hz.zhixingplan.top/gtdaqapeob.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtighgofpm.html

JS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gthniayqnr.html

TS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtsfpyjvng.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zdqjudy.top/gtlcabfuco.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtpyqggaxq.html

Ruby: s.reverse
来源：http://hz.yangfankeji.com/gtbtkvegdo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtqweggtor.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtoiwldpsf.html

Py:   s.count("a")
来源：http://hz.yueranfly.top/gtgqusuldj.html

PHP:  substr_count($s, "a");
来源：http://hz.zhixingplan.top/gtyqhrmigx.html

JS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtwcnoxszd.html

TS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtjuzybghs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuetiantiany.cn/gtqicelmaq.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtnjgozvlq.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtumuhxxac.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jyoumei.cn/gtypxlowcy.html

[E13] 逐字符遍历
来源：http://hz.feifeiyinyue.top/gtxdjlzoyl.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gtcxeakkdz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtjauwocbm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtrgztkkhh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtqboacbuk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gtvnvbnedp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.kuanghao11.cn/gtavlmcszi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.havefunace.top/gtpeuznhut.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.feifeiyinyue.top/gtdsgmfkgx.html

[E14] URL 编码与 Base64
来源：http://hz.quarkkingdee.top/gtjghevyoz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xinyue.icu/gtvoewohfw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zycfv.cn/gtalydixoq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ppjwa.cn/gtmbzqmjmv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sufxvd.cn/gtnycivsqq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj202588.top/gtljdovscu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hywenlv.cn/gtuayyqjpl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtycxgucju.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtbonrxsfe.html

[E15] HTML 转义 / 反转义
来源：http://hz.9152youxi.cn/gtltvztjnl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtfstawphn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ywan-chungtsiang.top/gthomguoij.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gzhubu.top/gtjjpcvmrp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtnrlclwud.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.snrcjt.cn/gtsihdeslt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigfzy.top/gtbthvjxnh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ppjwa.cn/gtijssvkkh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yangfankeji.com/gtaufnchcq.html

[E16] 数字千分位
来源：http://hz.nanxuanxn.top/gtzbqemvfj.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtxmisdtgj.html

PHP:  number_format(1234567);
来源：http://hz.chenjidiqi.icu/gtgghenknc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtummhoscp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtixvaspll.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtsyiwemep.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shangyingyoupin.top/gtonptmiwh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tanke756.top/gtgbtgeukc.html

C#:   1234567.ToString("N0")
来源：http://hz.zhoulong.xyz/gttckhhhzr.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtorklzzib.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tianlin.xyz/gtqcaganpl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.fzhhl.top/gtagwsisjl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtbyzhafhv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zycfv.cn/gtyuyxzgwa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hysaishi.cn/gtfmbdntey.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.haohaochexian.top/gtxuvhkbps.html

Ruby: s.capitalize
来源：http://hz.xziqi.cn/gtuoyvjtun.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jyoumei.cn/gtqpndatmz.html

[E18] 模板占位符替换
来源：http://hz.hywenlv.cn/gtxwvxtnum.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dashuyun.cn/gthomncbtj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gtlhprzhpx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtnkntxspd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtumhcgijq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guowangkeji.top/gtcfpzyffj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gzhubu.top/gtzxuenhbg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtqaoahudv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtpzohaubr.html

[E19] 多行文本按行拆分
来源：http://hz.zdqjudy.top/gtfhfskhiy.html

Py:   s.splitlines()
来源：http://hz.yj20258888.top/gtocyjxkkx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxinkj.top/gtbhytnyit.html

JS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtypbdcaze.html

TS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtvmkltcqs.html

Java: s.lines().toList()
来源：http://hz.zhongyouzk.top/gtzxdzbypy.html

Go:   strings.Split(s, "\n")
来源：http://hz.hysaishi.cn/gtztfivdqr.html

Ruby: s.lines
来源：http://hz.zhaomingkeji.xyz/gtpqveodaw.html

C#:   s.Split('\n')
来源：http://hz.xinyue.icu/gtvmmwrkaz.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtekvczcbj.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtxlcshiup.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dianchejie.cn/gtraqbajgb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydjk.org.cn/gtawfyqnpr.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gtsihulpku.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtoewssbmv.html

Go:   if s == "" {}
来源：http://hz.yj20258.top/gtkgruferd.html

Ruby: if s.empty?
来源：http://hz.hywenlv.cn/gtwexrmjbp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtqhwglyge.html

[E21] 超长截断加省略号
来源：http://hz.c1oappe.top/gtrwbhbexr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ppjwa.cn/gtmmcouzou.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtvwbeoyjo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtnbrfvpyz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtgzoiglxn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtjhebfjha.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxuanxn.top/gtylndnbrf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigufen.top/gtbhbckhzc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtxnajontl.html

[E22] 字节长度与字符长度
来源：http://hz.xuetiantiany.cn/gtvqwvyjlt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtaiqeyhik.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtecunlsgp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtkcpbzdur.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtazdjdbny.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gttfeyzwmp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zdqjudy.top/gtzjtjqmgi.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtjpxdhmqm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gtypajhmbx.html

================================================================================
来源：http://hz.9152youxi.cn/gtzlmaasun.html

F. 文件与目录
来源：http://hz.shanyushiyangkeji.top/gtyyercyhb.html

================================================================================
来源：http://hz.aibaodan.cn/gtevvlhvox.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gttgkfpqox.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtocpvhfnj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gtrvydpzjx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gtznylnnvz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guannengcc.top/gtriobtczw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtbrtigcgn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xylfe.cn/gtzfjlnmjb.html

Ruby: File.read("a.txt")
来源：http://hz.ppjwa.cn/gtisqfnnfl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gtoxtdecbp.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtihcchytr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.smart0.xyz/gtyvphoxvm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.316326.xyz/gtqtleadam.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtyrtwlpoz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gteplamgdc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtcdwcgzmo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.9152youxi.cn/gtpnlahtye.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gtvcdomqou.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtbzcjrzkw.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtrllaitmv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.52xcode.cn/gthqqmkmng.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtittsfcpl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtdnlzuroz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtpdehrghl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtvmmhwvmd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.andypj.xyz/gtvfwlcyyx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuanzhike.top/gtmysxpbsh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fengsongda.top/gtzmkztecp.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtcleaufan.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yanxiufei.cn/gtptjpbqdc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.redwolf501.top/gtlriirptd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnqzz.top/gtrnpjhedg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtlbgsiiqg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.andypj.xyz/gthmahhtct.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtxtlintsv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gaohongyu789.top/gtgrschdrc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtdsqrvfbl.html

[F05] 判断文件或目录是否存在
来源：http://hz.birdmap.top/gtghqbnbaj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtkvlmgekn.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtrchjamao.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtulffncra.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtqlinyglw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtwjgxfbem.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gtkxvxkkcx.html

Ruby: File.exist?("a.txt")
来源：http://hz.birdmap.top/gtebkaarjd.html

C#:   File.Exists("a.txt")
来源：http://hz.ydzc1.top/gtzzxdprsm.html

[F06] 删除文件
来源：http://hz.andypj.xyz/gttctkzhmv.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtnheriaws.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gtgppshrgv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtzmglkqcc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtpzbszffe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtpwqnotig.html

Go:   os.Remove("a.txt")
来源：http://hz.hywenlv.cn/gtvwkztupl.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtqunwldhy.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gtxbjmcecd.html

[F07] 创建目录（含多级）
来源：http://hz.hongshengwenyu.top/gtsotmhmlg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.andypj.xyz/gtgrkqzydk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.aibaodan.cn/gtbuhppuam.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gtdoauezjk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtnvqxsycv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gzhubu.top/gtqckdcmpg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ivvv.top/gtdsopazho.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtokdfyxqz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.smart0.xyz/gtofejenqm.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gtgifspzjv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtibivacmz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhongyouzk.top/gtlqfszjlk.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gttoxgfnmv.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtiqwmogrq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtzonscuae.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj202588.top/gtmbtldvfy.html

Ruby: Dir.children("dir")
来源：http://hz.wangdashe.top/gtqpxeljko.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtkymkxvyr.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gtsvbpwtpo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtmaltsapn.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtjyepxucj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtjljnxczw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtljafficu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtpodujkuq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.svipenyu.cn/gtcnjixalm.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtempabsev.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fzhhl.top/gteqbclmzk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtwtzfexnw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtmqkeawso.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yanxiufei.cn/gtlxinzagf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtjphatuav.html

TS:   path.extname("a.txt")
来源：http://hz.316326.xyz/gtfxuiouxf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dashuyun.cn/gtcxikdkck.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtrygyapuc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtnhqhaefy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.smart0.xyz/gthzvqdfsn.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtdqwgwqav.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtdsiedynp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgfzy.top/gtefpbldjq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtbgsvtmdz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtbwytrxfp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gtvdakjzet.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhixingplan.top/gtmpxlphql.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtdtntatbi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinyuanbaomall.cn/gtmempgovh.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtzdyazylg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yongpay.top/gtuoqjvsjk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtrdngfvdv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtgvoygivl.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtllgruelt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtnbzoagip.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hysaishi.cn/gtkbhasznj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenlongwang.top/gtvhywwtfn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtowgumens.html

================================================================================
来源：http://hz.smart0.xyz/gtnyfrtqla.html

G. 面向对象
来源：http://hz.yj20258.top/gtvfiupiau.html

================================================================================
来源：http://hz.gogol.net.cn/gtdbrzknos.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtbwpaemxb.html

Py:   class User: pass
来源：http://hz.xinyue.icu/gtnfghhnkp.html

PHP:  class User {}
来源：http://hz.jqgufenzy.top/gtnxzvtjif.html

JS:   class User {}
来源：http://hz.hammf.cn/gtsgjuqonr.html

TS:   class User { name: string = ""; }
来源：http://hz.guowangkeji.top/gtwcbgbujy.html

Java: class User {}
来源：http://hz.yonumen.top/gthrprondm.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtpsiqucoz.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gtxkqoexkf.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtsnkpzcnx.html

[G02] 构造函数
来源：http://hz.xingfuxueyuan.xyz/gtvgspbwpi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenjidiqi.icu/gtdmffoyem.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtmuoeynwe.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtdcvkjeik.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258888.top/gtsorltlbk.html

Java: User(String name) { this.name = name; }
来源：http://hz.iojbl.cn/gtkbeuaoog.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtuwqvaldv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtaivjyfyl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtmkqudarg.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtcyqlwufb.html

Py:   self.name = "x"
来源：http://hz.aibaodan.cn/gtgvngxudn.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtqkusccls.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtrpshhcpm.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtcwuckjrs.html

Java: private String name;
来源：http://hz.mhx1999.top/gtmslprhhm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gturqpvglh.html

Ruby: @name = "x"
来源：http://hz.yj202588.top/gtylmrlnpc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gthujyfvvo.html

[G04] 定义方法
来源：http://hz.jlsjyb.cn/gtgglkafbi.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtukgxvznr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtlzbvrbua.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtygswijwo.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gteekeufzb.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtycieirch.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cashguo.top/gtrxuwqqts.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtavdsbiks.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtzkhvainf.html

[G05] 继承
来源：http://hz.bjfxy.top/gtgimdasvd.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gthehhibto.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gtqypshhda.html

JS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtsisnzzcv.html

TS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtdccpjbex.html

Java: class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtbnmggzfn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ybcxt.top/gtkdwkabya.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtuaoecyzy.html

C#:   class Admin : User {}
来源：http://hz.svipenyu.cn/gtaavimhxd.html

[G06] 重写方法
来源：http://hz.sysykeji.top/gtadlnujgq.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtodutxkzd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtrmpbnsam.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtoimnayyk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtpsstazpz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtcmqalmnx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ywan-chungtsiang.top/gtsaqvhbjp.html

Ruby: def greet; "admin"; end
来源：http://hz.aibaodan.cn/gtrgffutgr.html

C#:   public override string Greet() => "admin";
来源：http://hz.jyoumei.cn/gtemokgfcn.html

[G07] 调用父类方法
来源：http://hz.hnxiangtu.top/gtndnouftc.html

Py:   super().greet()
来源：http://hz.52xcode.cn/gtfrjsjubl.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtupypdkiz.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtujtfsbfl.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtclqjbemj.html

Java: super.greet();
来源：http://hz.ydjk.org.cn/gtqbnpswcg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.redwolf501.top/gtofjyqhpn.html


<!-- 参考信息 -->