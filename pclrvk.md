代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pycfn.com/gtaayslgcx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangdashe.top/gttdzjbzdh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ehwqpu.com/gtnoarigkl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cqqwz.cn/gttzaxryka.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtkhggzsqv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cucudq.cn/gtxuutypwb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtqgtjakdl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gzhubu.top/gtebgubacf.html

[E06] 替换子串
来源：http://hz.xuetiantiany.cn/gtraszxcxr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.smart0.xyz/gtsgwwnxbo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yvedp.cn/gtpqfdxnyn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtikybovwl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtsynljvcg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtpktuvggg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gtynmanzsj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxuanxn.top/gtlsbvmraa.html

C#:   s.Replace("a", "b")
来源：http://hz.shzxlz.cn/gtcqxiblyz.html

[E07] 按分隔符拆分
来源：http://hz.dashuyun.cn/gtbugdrsqh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.316326.xyz/gtnndhbqti.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pycfn.com/gtibtrjjzy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sysykeji.top/gtwawjflqw.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtmjjywhyi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nwbrower.top/gtctlijbuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.vqdsnc.cn/gtzxjxrole.html

Ruby: s.split(",");  s.split
来源：http://hz.shuidangran.top/gtcqspjepa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aibaodan.cn/gttrgpxxte.html

[E08] 数组按分隔符合并
来源：http://hz.ydjk.org.cn/gtjaqylfoz.html

Py:   ",".join(items)
来源：http://hz.yvedp.cn/gtutthagrw.html

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gtuzwfgbpz.html

JS:   items.join(",")
来源：http://hz.guannengcc.top/gtkrdqdool.html

TS:   items.join(",")
来源：http://hz.xinyue.icu/gtxiadjqmz.html

Java: String.join(",", items)
来源：http://hz.gogol.net.cn/gtlqpzghrq.html

Go:   strings.Join(items, ",")
来源：http://hz.shuidangran.top/gtijqukyix.html

Ruby: items.join(",")
来源：http://hz.shuidangran.top/gtxmuqtvyv.html

C#:   string.Join(",", items)
来源：http://hz.gogol.net.cn/gtxyufbeov.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gtjukdlhgz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.vqdsnc.cn/gtmtrvkudh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtpwvsajit.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtinwzampf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtfgyxnrne.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.andypj.xyz/gtghkxqxbe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtjtqinwkg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yongpay.top/gttcauqxmw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtymonxvan.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtfpshpqyh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhixingplan.top/gtxwqhxduc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtcxwtwqwl.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtjbzqiyfp.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtnynwqlmw.html

Java: String.format("%03d", 7)
来源：http://hz.sysykeji.top/gtyfgjetyo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guannengcc.top/gtxwrcqqgj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtdpljzvbk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fzhhl.top/gtdeuldqeg.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtbufgnjra.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gtzfdjjmnc.html

PHP:  strrev($s);
来源：http://hz.zdqjudy.top/gtcveoylmv.html

JS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtnznfyxzo.html

TS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gttufjjvri.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cashguo.top/gtdzvrkjtj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ehwqpu.com/gtvexfadtb.html

Ruby: s.reverse
来源：http://hz.nanxinkj.top/gtyyrdcgae.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtnbtqcsuw.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangtech.top/gtenlmsanw.html

Py:   s.count("a")
来源：http://hz.shuidangran.top/gtbfxlfgcx.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gteijseabh.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtjzwbptrp.html

TS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtaigsfrio.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aibaodan.cn/gtlranetfg.html

Go:   strings.Count(s, "a")
来源：http://hz.zhijiandao.cn/gttjncycvb.html

Ruby: s.count("a")
来源：http://hz.jinqigfzy.top/gtvzqgaogm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gtqzrimzej.html

[E13] 逐字符遍历
来源：http://hz.bjfxy.top/gtqdnpiyzn.html

Py:   for ch in s: print(ch)
来源：http://hz.ivvv.top/gtypkvvqwm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jiagoushi.top/gtlbenmgtr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtmqfjuija.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtkgepoqxl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.c1oappe.top/gtscqqqclb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtbqqieruf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yangfankeji.com/gtjgdxazvf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.chenlongwang.top/gtlkxmkqhv.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gtiorzbewn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhengqikj.top/gtawvcdxfc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cqqwz.cn/gtrxbwtehk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtvfgjszvx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.9152youxi.cn/gtdkwhtvqc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtilhthspe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gttjavglqy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cqqwz.cn/gtlzvwtncz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhongyouzk.top/gtdcoigjyk.html

[E15] HTML 转义 / 反转义
来源：http://hz.yonumen.top/gthcuzazwi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangkeji.top/gtsscayoup.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.9152youxi.cn/gtgdlrgges.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cashguo.top/gtckezcwcn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtsvhaklag.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gtohjuyyfl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ybcxt.top/gtijkkyjzs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtnjfynito.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guowangkeji.top/gtbdigehsl.html

[E16] 数字千分位
来源：http://hz.fengsongda.top/gtpjztwdyw.html

Py:   f"{1234567:,}"
来源：http://hz.iojbl.cn/gtobcrsrhn.html

PHP:  number_format(1234567);
来源：http://hz.vqdsnc.cn/gtymuazwya.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtbotgnddu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtjxqxdgbm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtpagzgced.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ppjwa.cn/gtlzfttssd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gaohongyu789.top/gtizxodjma.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtptcsmhyc.html

[E17] 首字母大写
来源：http://hz.xuanzx.com/gtqxmggxyb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gzhubu.top/gtxunwssou.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gteqwmivyg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gttzehaqpa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtwltiuxuu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sxryk.cn/gteljcluug.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtkbvujndb.html

Ruby: s.capitalize
来源：http://hz.9152youxi.cn/gthiyxrgna.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aizwys.cn/gtlfucvfth.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtxkldjhwq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtdmgqzeco.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258888.top/gtyxtfgpbl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtqqkdkcpa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtpuclveab.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhengqikj.top/gtlgmnmcqc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yanxiufei.cn/gtkxwrpmqu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtzbgxyhqn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtjrufkpch.html

[E19] 多行文本按行拆分
来源：http://hz.redwolf501.top/gtvbtztlov.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gtheznwqtz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hammf.cn/gtshuopeen.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtrhaewufd.html

TS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtfxasntue.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtqoqvzgja.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gttdkydsxr.html

Ruby: s.lines
来源：http://hz.shanyushiyangtech.top/gtszxceffd.html

C#:   s.Split('\n')
来源：http://hz.0kj1m.cn/gtoztouxuc.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gtgngjvzka.html

Py:   if not s:
来源：http://hz.ppjwa.cn/gtkmstdpjg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dashuyun.cn/gtdghtgujb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtpfyksztv.html

TS:   if (s === "") {}
来源：http://hz.mhx1999.top/gtrgwxwwmy.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtfmzpqihz.html

Go:   if s == "" {}
来源：http://hz.0kj1m.cn/gtwfyjilxp.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtnftwfbmr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sufxvd.cn/gtlbyhbfkw.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtvfyqlvxv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgfzy.top/gtljqqhoxw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.smart0.xyz/gtaaxvtlik.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gthfuobuti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtdspegzol.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtpxaupwex.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtzldjrgpv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gthiyuaion.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtbhskzfhg.html

[E22] 字节长度与字符长度
来源：http://hz.jqgfzy.top/gtbabmrjnf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnqzz.top/gtdtjsmrur.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtnrwtiapm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtuhbknhll.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtfzjnfvxs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gtcoheyqnn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hongshengwenyu.top/gtbqqjuwmx.html

Ruby: s.bytesize;  s.length
来源：http://hz.52xcode.cn/gtimgbzutj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gtgdauzkll.html

================================================================================
来源：http://hz.xylfe.cn/gtxdbuuzzi.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtabxonewx.html

================================================================================
来源：http://hz.xylfe.cn/gtjtvoauey.html

[F01] 读取整个文件
来源：http://hz.yonumen.top/gtzetjszvp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pycfn.com/gtdxtemaxx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gttlgfaqlz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nwbrower.top/gtznwrspiu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jiagoushi.top/gtzvlwgbcm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtptfveaxs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gtprqxdapi.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gtasqnlydq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nwbrower.top/gtrwzbnkpi.html

[F02] 逐行读取文件
来源：http://hz.guowangkeji.top/gtuwzjdfhr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tanke756.top/gtwuibpvdh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtjvnetvjw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtdtqnbnpp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtupnnqwbq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtujodwtsv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydjk.org.cn/gtmbcgyhna.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xziqi.cn/gtcpyoxaaw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtkycpipto.html

[F03] 写入文件（覆盖）
来源：http://hz.redwolf501.top/gtlonxhnoi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ehwqpu.com/gtpbtlbize.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtqbuvklqa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtiejflzrw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtjgbllpsl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhoulong.xyz/gtewoowhpi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cdnleiting.top/gtlsmczgdo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtdfayiing.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gtnslfbwpv.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtcxqzyihg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtcfyfirvj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtapsubhfe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gteplarirr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtioqrkxop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtsahdtyse.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtzjuypxrp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sufxvd.cn/gtusxaklce.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gtdxyjmepo.html

[F05] 判断文件或目录是否存在
来源：http://hz.dianchejie.cn/gtlushhakn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtmshqwnvx.html

PHP:  file_exists("a.txt");
来源：http://hz.feifeiyinyue.top/gtpbtgdaer.html

JS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtxjtpzqcf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtpcgljqmm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtllcjdmbt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gttewukzon.html

Ruby: File.exist?("a.txt")
来源：http://hz.cashguo.top/gtqimmqgkd.html

C#:   File.Exists("a.txt")
来源：http://hz.shzxlz.cn/gtmwfhgtmw.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtudxgraer.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtezjipsry.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtfrgyjcfg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtmafkwxea.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtkvufdohw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtxghjrwzs.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtuyxbcfor.html

Ruby: File.delete("a.txt")
来源：http://hz.havefunace.top/gtllpoueiz.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtixlfpwkw.html

[F07] 创建目录（含多级）
来源：http://hz.xuanzx.com/gtszdufxgk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ivvv.top/gtcmoximuq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtakbibjzr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtjmwdlsdv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtiruglpkv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pengpengdd.cyou/gtksroeolx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtuczgtbgv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258888.top/gttwndwfvt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zdqjudy.top/gtqeducmqo.html

[F08] 遍历目录
来源：http://hz.yanxiufei.cn/gtalxwdmsu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtqtknmcdt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtyehxtefj.html

JS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gthdnldgnu.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtsubklhsf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtmdflbujo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gtzdwmxisp.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtitlmyhgn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtnhzimatx.html

[F09] 获取文件大小
来源：http://hz.gogol.net.cn/gtpfzjhyjl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gzhubu.top/gtfwhbocrv.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtkiusnwrk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtgxomemat.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtfumqcdgh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtshpeuuax.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtgbqntcfy.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtrlgnouau.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.vqdsnc.cn/gtkjuumlcn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gtitxchqiw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtkxmmykzw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.haohaochexian.top/gtgiwbgioy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtrjlbmhtq.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gtnzhfidtn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gtksgvopjh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtawlkzivi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtocbgeeds.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shuidangran.top/gtotqvaguh.html

[F11] 复制与移动文件
来源：http://hz.ybcxt.top/gtdbrchhoo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtumqnnodb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhaomingkeji.xyz/gtwmdmzria.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gttwcnypcb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtpsxkcxrt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.smart0.xyz/gtlktyghlk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtemkedqgo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gttlmmmnda.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jlsjyb.cn/gtuvoeejak.html

[F12] CSV 读写
来源：http://hz.jqgufenzy.top/gtoujatqdh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gzhubu.top/gtpcommwwi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.quarkkingdee.top/gtxsikdeqc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtyxderchg.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gtjtyjwqyd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tianlin.xyz/gtibwzefhm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gtqzuhotzd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nwbrower.top/gtxshmocjo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtgxmsswyb.html

================================================================================
来源：http://hz.yongpay.top/gtlkkhigum.html

G. 面向对象
来源：http://hz.hnqzz.top/gtqomuihoz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtubqvbbjw.html

[G01] 定义类
来源：http://hz.yonumen.top/gtwlentprf.html

Py:   class User: pass
来源：http://hz.hammf.cn/gtzmigwboq.html

PHP:  class User {}
来源：http://hz.jqgufenzy.top/gtqntowaan.html

JS:   class User {}
来源：http://hz.guowangkeji.top/gtqaptbbpf.html

TS:   class User { name: string = ""; }
来源：http://hz.haohaochexian.top/gtanaybmbs.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtqjgqkdzd.html

Go:   type User struct { Name string }
来源：http://hz.pengpengdd.cyou/gtkttrvmcu.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtpldyescf.html

C#:   class User {}
来源：http://hz.shuidangran.top/gtxzmlvvhk.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtvsplakxi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gtdrgrhzfx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtqstksxal.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gthqznkxpd.html

TS:   constructor(public name: string) {}
来源：http://hz.dianchejie.cn/gtgobqvnfx.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtpjjcgusm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangtech.top/gtzyuwcodc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtzrajviuy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ybcxt.top/gtxnjtevmh.html

[G03] 实例属性
来源：http://hz.wangshuangyany.cn/gtnhbheyzd.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtvcdwdaup.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gtnrihugva.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtdaambprf.html

TS:   name: string = "x";
来源：http://hz.jianghu66.top/gteynaybzb.html

Java: private String name;
来源：http://hz.jianghu66.top/gttdqqvfxl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtpjqoyskc.html


<!-- 参考信息 -->