代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtxfsemauq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtmahwwaop.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj202588.top/gtchgfzfkw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yanxiufei.cn/gtmpwujclm.html

C#:   s.Replace("a", "b")
来源：http://hz.hysaishi.cn/gtblkwkfls.html

[E07] 按分隔符拆分
来源：http://hz.zhijiandao.cn/gttkrfligj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pengpengdd.cyou/gtjwpweogl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jiagoushi.top/gtbzayyjui.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jianghu66.top/gtbeuwmdmb.html

TS:   s.split(",")
来源：http://hz.tanke756.top/gtexnnqynz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pycfn.com/gtnpcveytj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydjk.org.cn/gtkmqnstdd.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangtech.top/gtxbiypknr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shanyushiyangkeji.top/gtncaeudln.html

[E08] 数组按分隔符合并
来源：http://hz.shanyushiyangkeji.top/gtnswfhggv.html

Py:   ",".join(items)
来源：http://hz.yvedp.cn/gtadvmktgs.html

PHP:  implode(",", $items);
来源：http://hz.zhixingplan.top/gtqqzrvnfn.html

JS:   items.join(",")
来源：http://hz.xziqi.cn/gtdbykhgtu.html

TS:   items.join(",")
来源：http://hz.cdnleiting.top/gtjmvzzmsf.html

Java: String.join(",", items)
来源：http://hz.yonumen.top/gtibgaviso.html

Go:   strings.Join(items, ",")
来源：http://hz.guowangkeji.top/gtbbrqdjld.html

Ruby: items.join(",")
来源：http://hz.feifeiyinyue.top/gtcsaskyqv.html

C#:   string.Join(",", items)
来源：http://hz.daxiang520.top/gtebmxzzet.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtxwqraweq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuanzx.com/gtpdyihqre.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gtnqrbjzqf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.vqdsnc.cn/gtldpgfzwh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtznivuhag.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daxiang520.top/gtgwamxoif.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jianghu66.top/gtjewgdejz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gtztoyquzi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gthmlpqbkf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gtkcdijzxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhiwuduotai.top/gtlcxmpazm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aibaodan.cn/gterxedmfc.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtddlieuyu.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtfjtzhzzl.html

Java: String.format("%03d", 7)
来源：http://hz.cucudq.cn/gtwwugbsru.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xylfe.cn/gttscibpiq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtxszayrvw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gthqcdlhpi.html

[E11] 反转字符串
来源：http://hz.zhongyouzk.top/gtigljxnuj.html

Py:   s[::-1]
来源：http://hz.tianlin.xyz/gtgeiksuld.html

PHP:  strrev($s);
来源：http://hz.kuanghao11.cn/gtsastjtbe.html

JS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtkijiucgi.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtcihhsvin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtfbkeffpu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tian-w.cn/gtmrjgglao.html

Ruby: s.reverse
来源：http://hz.nanxuanxn.top/gtznnjnzkn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtryuiykkh.html

[E12] 统计某字符出现次数
来源：http://hz.cucudq.cn/gtnkmxlaqm.html

Py:   s.count("a")
来源：http://hz.ydzc1.top/gtefzqbqgz.html

PHP:  substr_count($s, "a");
来源：http://hz.sufxvd.cn/gttwuzyefp.html

JS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtywhxnwmx.html

TS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtlnhvblak.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sxryk.cn/gtfvblnusp.html

Go:   strings.Count(s, "a")
来源：http://hz.316326.xyz/gtnrihyxsg.html

Ruby: s.count("a")
来源：http://hz.9152youxi.cn/gtgnjbkdpk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtkorornei.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gtpaswwcgu.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtfxjzztjb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuxming.cn/gtnjjxkwgl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtjqwqrnen.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtudywayme.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xinyue.icu/gttqnzidri.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.birdmap.top/gtrqwcrsdn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yonumen.top/gtejqaydsy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258.top/gtgwhyndmx.html

[E14] URL 编码与 Base64
来源：http://hz.aizwys.cn/gtwywjotqn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuanzhike.top/gtcycirvoo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jlsjyb.cn/gtwywtwqvz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhiwuduotai.top/gtwrdmpukk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangkeji.top/gtpbaydsel.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgufenzy.top/gtsxorxczw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zycfv.cn/gtknghtttk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtlejpqtxm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jlsjyb.cn/gtqxdoushp.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtngaxwxak.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tianlin.xyz/gtasgnwsax.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuxming.cn/gtcsyhkpas.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258888.top/gteelpikjl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnqzz.top/gtmdfaxhrh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtnsgkeydn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gtzrpudzkb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hammf.cn/gtwojjqugw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.52xcode.cn/gtgkbtvxxv.html

[E16] 数字千分位
来源：http://hz.jinyuanbaomall.cn/gtiphluflq.html

Py:   f"{1234567:,}"
来源：http://hz.gzhubu.top/gtwuylslro.html

PHP:  number_format(1234567);
来源：http://hz.jinghuilouyu.cn/gtbroekdzq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtjplgosfr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtyqhcaotm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xziqi.cn/gtesevznjo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.52xcode.cn/gtvwacmfra.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinyuanbaomall.cn/gtrlvblphz.html

C#:   1234567.ToString("N0")
来源：http://hz.sweek.top/gtogkvrwfm.html

[E17] 首字母大写
来源：http://hz.jiagoushi.top/gtgqjicclp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhengqikj.top/gtqlroykvg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtcqgrmsze.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtxmndjuna.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gtvfsjokfh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jlsjyb.cn/gtqxonvhbt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.haohaochexian.top/gtaequvlxz.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtrdffxtiq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.vqdsnc.cn/gtxbdfqqeo.html

[E18] 模板占位符替换
来源：http://hz.bjfxy.top/gtwjwpblbu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jiagoushi.top/gthamdkelu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gtpisfnnol.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtuphibdvy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtwnprjooj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuanzhike.top/gtgfsafeej.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dianchejie.cn/gtipdngdsi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cqqwz.cn/gttqrlfpmm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.guowangkeji.top/gtapokshxk.html

[E19] 多行文本按行拆分
来源：http://hz.shzxlz.cn/gtuuckykvg.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtigynitsg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhijiandao.cn/gtkgvczocq.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtkfzrcwmk.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtbhkwsffq.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gtuazgpppw.html

Go:   strings.Split(s, "\n")
来源：http://hz.nwbrower.top/gtqjteopwp.html

Ruby: s.lines
来源：http://hz.pengpengdd.cyou/gtglyyhydi.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gttnmvcqvu.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtxewjxriv.html

Py:   if not s:
来源：http://hz.52xcode.cn/gtgwgilkux.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cqqwz.cn/gthtzyuhlw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yangfankeji.com/gtjutvbper.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtwwyvpgej.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtiylccwrm.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtizjduqtn.html

Ruby: if s.empty?
来源：http://hz.yueranfly.top/gtnflfypqx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtsckyddbv.html

[E21] 超长截断加省略号
来源：http://hz.daxiang520.top/gtpkznzagf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yangfankeji.com/gtgejsvpqk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtlcqevhwx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtwksrequy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtvlwfpmta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtxrcepwkp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtywfuwukt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtwfjsxorc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtqnhvrlsi.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258888.top/gtdumcguzb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gtpcppdhtp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jiagoushi.top/gtiylcdilz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtruvaqtbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtzkkdfbxr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj202588.top/gtawagwnkq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dianchejie.cn/gtiaeriinw.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtodfeaybj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenjidiqi.icu/gtgynwgtpm.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnfwtrcxb.html

F. 文件与目录
来源：http://hz.sufxvd.cn/gtblacuprp.html

================================================================================
来源：http://hz.xziqi.cn/gtdvwphots.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtkpnamxsn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jyoumei.cn/gtlzmiswjn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtlyicvuvq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daria6918.cn/gtcvysmejh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gttotcwvzb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtqpedgruq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtbtcgfdvn.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gtcuponsbn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtdmaypobr.html

[F02] 逐行读取文件
来源：http://hz.pengpengdd.cyou/gtadppkpvy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ybcxt.top/gtbvnmggbo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sufxvd.cn/gtxrkhqjmy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtvlgrioke.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtrzpgmpss.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtrfwvgkqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtmuxlidsf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xuanzx.com/gtkwfpkkam.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtybevtjoo.html

[F03] 写入文件（覆盖）
来源：http://hz.tianlin.xyz/gtkvvxgaau.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jlsjyb.cn/gtpuyfbtbo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtbuvlhfwn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtxrrhcvlf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtzwuwtqwt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.havefunace.top/gtsjddqgdu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtqjoigxdi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zycfv.cn/gttyyeecfy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtfpdrgnus.html

[F04] 追加写入文件
来源：http://hz.yuxming.cn/gtkzilyuqf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shangyingyoupin.top/gtoguxljns.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtkzxomecc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtbznfstzi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtaeejknvt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhengqikj.top/gtakucdvbk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cashguo.top/gtyfkhbgxa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gtcpkcimkn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tanke756.top/gtrpwsweey.html

[F05] 判断文件或目录是否存在
来源：http://hz.shuidangran.top/gttihqksbq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.feifeiyinyue.top/gtaycfgvgf.html

PHP:  file_exists("a.txt");
来源：http://hz.gotoacloud.top/gtjivraehi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtnnpbzogz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtwqmzwihk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtdpowtohl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtwezdxkla.html

Ruby: File.exist?("a.txt")
来源：http://hz.feifeiyinyue.top/gtadrkndki.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigfzy.top/gtfvfsifaj.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtjvmafhvt.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtmuxvalgv.html

PHP:  unlink("a.txt");
来源：http://hz.yueranfly.top/gtfktfoasi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gttyyshxrp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtrwwspufi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtbhoxmkev.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtctsxxgeo.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gttbfpulcw.html

C#:   File.Delete("a.txt");
来源：http://hz.cheryme.top/gtuttwlmgv.html

[F07] 创建目录（含多级）
来源：http://hz.ybcxt.top/gtutthpkpf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtwjjkldlu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cheryme.top/gtaipxyfus.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtknegincw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtkuewpddx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gtaldgsinl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gzhubu.top/gtidirgggw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yonumen.top/gtqltecwvg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shuidangran.top/gtujqyrvfr.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtfovujfnp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gtnhxxlpol.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtlqhunxtf.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtpseeumta.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtjvrldmjw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtsdqqofeh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtwxomzvtg.html

Ruby: Dir.children("dir")
来源：http://hz.nwbrower.top/gtugjwdzan.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nwbrower.top/gtvsbmlrpq.html

[F09] 获取文件大小
来源：http://hz.yanxiufei.cn/gtnziuljur.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258.top/gttxeqzlcv.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gthzxsfhbf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtwclisdjc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtnyzunjne.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gttmbrzrcl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nwbrower.top/gtsmczpqyr.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtagsbvhiw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenlongwang.top/gttxpqafcx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtkhnqmxbx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gthwyitbxk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigfzy.top/gtubbbmglk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtautftqfu.html

TS:   path.extname("a.txt")
来源：http://hz.316326.xyz/gtpnobhmup.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.9152youxi.cn/gtsuipqtpp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtwpvcjtoj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtotxdvste.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtpcgtdbyd.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtdkfgmmoj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gticnsuagx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtwxxvojfn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtxyfcsicm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtrhetnsnp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtcgkiixis.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zycfv.cn/gtredtfwxj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtxquhckmj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtqnhcjabv.html

[F12] CSV 读写
来源：http://hz.jlsjyb.cn/gtienmykuh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtqwcdkpfq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daria6918.cn/gtddlsmkae.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtwiunjhtv.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtsapeckxi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenjidiqi.icu/gtnagqorku.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangshuangyany.cn/gtpccukzpw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenlongwang.top/gtvliclbju.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhongyouzk.top/gtwkhvgldt.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrzrihonp.html

G. 面向对象
来源：http://hz.svipenyu.cn/gtfnmxtlxk.html

================================================================================
来源：http://hz.c1oappe.top/gtqaqoazvi.html

[G01] 定义类
来源：http://hz.shanyushiyangtech.top/gtuiwlycza.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtjvawwmcg.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtckjxxdep.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gthrlcwdcm.html

TS:   class User { name: string = ""; }
来源：http://hz.dianchejie.cn/gtaouzifod.html

Java: class User {}
来源：http://hz.xylfe.cn/gtnjmdwftc.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtfyarxsjt.html

Ruby: class User; end
来源：http://hz.shuidangran.top/gtrdtkqene.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gthqhfwrqw.html

[G02] 构造函数
来源：http://hz.snrcjt.cn/gtvoiucfdl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.c1oappe.top/gthxotrxuf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.52xcode.cn/gtwudjfgom.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gtxaoryivg.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtnmtwcwax.html

Java: User(String name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtlprezuyh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtggtoyovs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hywenlv.cn/gtomhyrvas.html

C#:   public User(string name) { Name = name; }
来源：http://hz.kuanghao11.cn/gtsdtndpkc.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtefwpngwr.html

Py:   self.name = "x"
来源：http://hz.cashguo.top/gtfcxrzgji.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gtbjauqugj.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtpuryjyyz.html

TS:   name: string = "x";
来源：http://hz.yuanzhike.top/gtlcpglbwx.html

Java: private String name;
来源：http://hz.wangdashe.top/gtmolqnkvm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pycfn.com/gtyewerxwz.html

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gtlcozbxjt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtcigaicra.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtcohudayj.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gtsfdlyszr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtonsnbcjz.html

JS:   greet() { return this.name; }
来源：http://hz.xylfe.cn/gtrdmgcqyd.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gttdjbfncc.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtbxdfocjn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtujjgwsvc.html

Ruby: def greet; @name; end
来源：http://hz.jqgfzy.top/gtreygipqj.html

C#:   public string Greet() => Name;
来源：http://hz.fengsongda.top/gtvnwyghdc.html

[G05] 继承
来源：http://hz.sweek.top/gtpvdozxct.html


<!-- 参考信息 -->