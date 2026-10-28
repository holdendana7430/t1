代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtyqkurcfq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.andypj.xyz/gtzkqgqvul.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtknwucoru.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ywan-chungtsiang.top/gtfekoysna.html

[E06] 替换子串
来源：http://hz.pycfn.com/gtegtwxqoy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gaohongyu789.top/gtnxaskest.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jyoumei.cn/gtchssfefu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtwmlosgfb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtkxudwjmp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtdhurfcvc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dashuyun.cn/gtqcgzsdpx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydzc1.top/gttfnzcsab.html

C#:   s.Replace("a", "b")
来源：http://hz.shuidangran.top/gtsedzabfo.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gthznkbgzy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258.top/gtrfkekzci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtiqxmbhjk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nwbrower.top/gtxeengubm.html

TS:   s.split(",")
来源：http://hz.dashuyun.cn/gtlxbrvtex.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.snrcjt.cn/gtbyaqufuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shangyingyoupin.top/gtnjsbqxbx.html

Ruby: s.split(",");  s.split
来源：http://hz.iojbl.cn/gtkufjafiz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhixingplan.top/gtryxtkyzt.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtmzmksylg.html

Py:   ",".join(items)
来源：http://hz.ehwqpu.com/gtidsnqxfz.html

PHP:  implode(",", $items);
来源：http://hz.xingfuxueyuan.xyz/gtozlqacau.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtppvswaij.html

TS:   items.join(",")
来源：http://hz.hysaishi.cn/gtasraaaaz.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gtioipscub.html

Go:   strings.Join(items, ",")
来源：http://hz.316326.xyz/gtcmkkibaq.html

Ruby: items.join(",")
来源：http://hz.hongshengwenyu.top/gtzmoozxum.html

C#:   string.Join(",", items)
来源：http://hz.xylfe.cn/gtwpmqmcei.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtpovvyphj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sweek.top/gtisyzijzp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtqrongolz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtwgdftjso.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yvedp.cn/gtfnlyjzcw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangdashe.top/gtlnfrrdlf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.9152youxi.cn/gtjaubkdia.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinyuanbaomall.cn/gtulzxbhok.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gtduqvvpje.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtlenojopx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sxryk.cn/gtqvriibud.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gtltybqrbr.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtnnprhznz.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtmijalkbt.html

Java: String.format("%03d", 7)
来源：http://hz.zycfv.cn/gtfmxzgbmc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ivvv.top/gtegfhdddo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtvmsssovt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtpskpdsoo.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtjxhwfnnn.html

Py:   s[::-1]
来源：http://hz.jlsjyb.cn/gtmsivdtfk.html

PHP:  strrev($s);
来源：http://hz.guowangkeji.top/gtkiiggfnp.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtgnulziox.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtdfkycioz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtuoffhkim.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtsrflngeg.html

Ruby: s.reverse
来源：http://hz.pycfn.com/gtpwarrfok.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtpzdyhryn.html

[E12] 统计某字符出现次数
来源：http://hz.zhixingplan.top/gtjboxaqkx.html

Py:   s.count("a")
来源：http://hz.shangyingyoupin.top/gttqbltndg.html

PHP:  substr_count($s, "a");
来源：http://hz.sweek.top/gtvajewkxk.html

JS:   s.split("a").length - 1
来源：http://hz.meibo888.top/gtnwpgrode.html

TS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gtkrythuhn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtriaufjzz.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtswrxowfb.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtjkpdrqdc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenjidiqi.icu/gtaekmdcqk.html

[E13] 逐字符遍历
来源：http://hz.feifeiyinyue.top/gtiytvmmrk.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gtmybdqmki.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuxming.cn/gtiqeinjgz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cqqwz.cn/gtffhdztoy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtcjdnelwu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangdashe.top/gtlfzjhufb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.andypj.xyz/gtvwrxepno.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtoyeiijcl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xylfe.cn/gtztuagzub.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtfncxrmcd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258888.top/gtlndsphso.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gtbclhtxaw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gtijomnehl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cheryme.top/gtssptlgmw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gtymkglnpi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtuhyjyynw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gthpnzksok.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgufenzy.top/gthydwaeho.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtlwuahdbe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenjidiqi.icu/gtdqtcsmjc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hammf.cn/gtwystzdyr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gteedulemn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yueranfly.top/gtcqjeohgb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gogol.net.cn/gtphfqwfng.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtwqvseiss.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtwceizukm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jianghu66.top/gtukxvqjca.html

[E16] 数字千分位
来源：http://hz.hongshengwenyu.top/gtrcllfunp.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gtiualmrkw.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtwhaawene.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtetzfbczb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtikpxxrxs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dashuyun.cn/gtlplypuhf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtpiekbqbi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dianchejie.cn/gtasbhaaoj.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigfzy.top/gtfnluunwy.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtiqwnsute.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtrxyxjokg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jyoumei.cn/gttboewnus.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtspfjoivy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gtwotvtbwg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cucudq.cn/gtchmnawps.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxuanxn.top/gteojkgrky.html

Ruby: s.capitalize
来源：http://hz.wangdashe.top/gteelernqs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gogol.net.cn/gttslhldxo.html

[E18] 模板占位符替换
来源：http://hz.hnxiangtu.top/gtxqdwugmj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jyoumei.cn/gtiwhtfjxk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yanxiufei.cn/gttxygxqkz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtbgiicyjy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gthbuuxmsb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuetiantiany.cn/gtqzvjxxzx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhengqikj.top/gtnlorjzbz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ehwqpu.com/gttentngbr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258888.top/gtezfdphtf.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gtuvfgymtq.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gteculdpfs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hongshengwenyu.top/gtpyvlbqbu.html

JS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtoffhhupy.html

TS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtpfnnpnxk.html

Java: s.lines().toList()
来源：http://hz.yvedp.cn/gtpfxvpgkr.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtpkphzkgq.html

Ruby: s.lines
来源：http://hz.nanxinkj.top/gtanzefdxg.html

C#:   s.Split('\n')
来源：http://hz.andypj.xyz/gtnshjwuie.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtsboemqja.html

Py:   if not s:
来源：http://hz.nwbrower.top/gtzditloyi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.vqdsnc.cn/gtxaxtxhpu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hysaishi.cn/gthpbgkhpq.html

TS:   if (s === "") {}
来源：http://hz.dianchejie.cn/gtznfgazqh.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtvjkuvfdr.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gttyspnqhh.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtdiwwttwq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ivvv.top/gtkcxxfish.html

[E21] 超长截断加省略号
来源：http://hz.jlsjyb.cn/gtxeigpkvz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxuanxn.top/gtmztqvohl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtnfupovgb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtnwtdchiu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtfgxgklkm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtcbroeitz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ywan-chungtsiang.top/gtxattipix.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jyoumei.cn/gtbrpiocti.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jiagoushi.top/gtkpetctjo.html

[E22] 字节长度与字符长度
来源：http://hz.aibaodan.cn/gtjdjjnbao.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigufen.top/gtpupjghsj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtijddsllx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtqthfkjru.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtzqemplla.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhixingplan.top/gtvyyfgrcs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhijiandao.cn/gthcqtukor.html

Ruby: s.bytesize;  s.length
来源：http://hz.jyoumei.cn/gtorhcbydp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtolyxslry.html

================================================================================
来源：http://hz.jiagoushi.top/gtffypecin.html

F. 文件与目录
来源：http://hz.fzhhl.top/gtwllfdqit.html

================================================================================
来源：http://hz.sufxvd.cn/gtvwhdthjy.html

[F01] 读取整个文件
来源：http://hz.zdqjudy.top/gtfybwpoec.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtvjticuzo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtjsppztkm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shzxlz.cn/gtvumdbycs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.52xcode.cn/gtoppfkndo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtnpnkqlfk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xinyue.icu/gtropvbyfr.html

Ruby: File.read("a.txt")
来源：http://hz.kuanghao11.cn/gtbowjncoq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cheryme.top/gttpkvhnid.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangkeji.top/gtmdwyjrgm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtrgxrwryk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtterpsvcs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtirircbdd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.mhx1999.top/gtsllatjes.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tianlin.xyz/gtebtzhecd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hongshengwenyu.top/gtdiheomyt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtqedhrjwp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtqderzypd.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtpciakxgl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtkfhvcbvl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtripvrtcf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gtorshahfa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtaydysgmm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtklpzcslu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258.top/gtqishsqqg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtdtetgqec.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtaabjjivl.html

[F04] 追加写入文件
来源：http://hz.yueranfly.top/gtnuxxhxar.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhaomingkeji.xyz/gtowogkxjo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gtuhozqaga.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtqemhioer.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtfffogyid.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gtqruubfbh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtbgmruorx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yangfankeji.com/gtbkteisri.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuanzx.com/gtajogsjoa.html

[F05] 判断文件或目录是否存在
来源：http://hz.316326.xyz/gtqmgdknwy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtfhtsppgb.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgufenzy.top/gtxvmncypr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtgtztigvb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtbjaacvjy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtuxkclcqz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hywenlv.cn/gtawhwdblb.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtxbtnmihj.html

C#:   File.Exists("a.txt")
来源：http://hz.shuidangran.top/gteyyfmayr.html

[F06] 删除文件
来源：http://hz.wangdashe.top/gtjwleihqq.html

Py:   os.remove("a.txt")
来源：http://hz.ehwqpu.com/gtvsapzsla.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtrjorgszu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtzsxvrwik.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtazrkzner.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtqmjumrpt.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtyivvmprk.html

Ruby: File.delete("a.txt")
来源：http://hz.yangfankeji.com/gtxgmcbibf.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtwbgyshab.html

[F07] 创建目录（含多级）
来源：http://hz.hnqzz.top/gtsnkupnek.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xinyue.icu/gtitdbhlbl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.birdmap.top/gtlvrlioda.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtrlsyhhwu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtotivvivj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtbycjioxq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinghuilouyu.cn/gtrmwnldkn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenzaomai.com/gtbbanqkdb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jyoumei.cn/gtgzntgqhl.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gtfozoivkt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cdnleiting.top/gtsdczgbzy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xinyue.icu/gtiwgszwie.html

JS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtxnrowcmr.html

TS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtxejgoslx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtvzqjdeda.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtmglmbfxi.html

Ruby: Dir.children("dir")
来源：http://hz.316326.xyz/gttpjbfvlg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhaomingkeji.xyz/gtcwgihtcx.html

[F09] 获取文件大小
来源：http://hz.nanxinkj.top/gtswyzxwzg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yongpay.top/gtvfnjdeam.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtzzxcuwnc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtabaxkhkq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtoaxyztbl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtnkgthyed.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.52xcode.cn/gtglizevqy.html

Ruby: File.size("a.txt")
来源：http://hz.jianghu66.top/gtiejbfcaa.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zycfv.cn/gtdvlnmpqm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhiwuduotai.top/gtnxclxnta.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtyzlslsaq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.feifeiyinyue.top/gtzixelyvd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gthlkmwlbe.html

TS:   path.extname("a.txt")
来源：http://hz.jiagoushi.top/gtazgxestr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtzpzqlcsp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gtygsforrk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtcaihyfyp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtpzuvqnib.html

[F11] 复制与移动文件
来源：http://hz.yangfankeji.com/gtpobnrtrg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtsdekdwfr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtvpnxuzgf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtosdxgcqc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtmvucsvzw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.feifeiyinyue.top/gtbecjqvcm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtngkqcdxx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtqjigcwbv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtgwhljeup.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtbdavcyyt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gtfsirezlb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtvzokxchq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gttrnzdjgk.html

TS:   // 同上
来源：http://hz.yvedp.cn/gtljsfpjeq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jiagoushi.top/gtdbynyzxm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtokyovpac.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhijiandao.cn/gtjziiatcf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtnekusvqp.html

================================================================================
来源：http://hz.daxiang520.top/gturszncrn.html

G. 面向对象
来源：http://hz.jlsjyb.cn/gtwkqlvdsf.html

================================================================================
来源：http://hz.sweek.top/gtejyaicxa.html

[G01] 定义类
来源：http://hz.jiagoushi.top/gtddeyuhhu.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtluxpwwcm.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtbnpjetuc.html

JS:   class User {}
来源：http://hz.jlsjyb.cn/gtvmkmaquq.html

TS:   class User { name: string = ""; }
来源：http://hz.shzxlz.cn/gtezhttqvg.html

Java: class User {}
来源：http://hz.ivvv.top/gtrgqptaht.html

Go:   type User struct { Name string }
来源：http://hz.yj20258.top/gteselqeov.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtlvqvbfws.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtkqxbmpkz.html

[G02] 构造函数
来源：http://hz.ivvv.top/gtzftqsfoy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtmbhtotne.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtqhuzbkry.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gtahcxfkuk.html

TS:   constructor(public name: string) {}
来源：http://hz.jinghuilouyu.cn/gtyqaviezw.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtkzufdaqf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtoearazyw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tian-w.cn/gtxcjvgnqs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gtsgrbzvqe.html

[G03] 实例属性
来源：http://hz.snrcjt.cn/gtjyqcoxdb.html

Py:   self.name = "x"
来源：http://hz.hysaishi.cn/gtdrjawthd.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtqxoegjrv.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtdxahpykb.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gtfmrzqitb.html

Java: private String name;
来源：http://hz.9152youxi.cn/gtdfpghmcq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtoljirycf.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtknrjmjeb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxinkj.top/gtgntmktfi.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gthlwzuxfk.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gtmhjeszwy.html


<!-- 参考信息 -->