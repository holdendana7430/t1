代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnxiangtu.top/gtvwmbowmn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtayzjiypf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtsobeqddx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gthlzvnzpm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gttolnfdfc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtjckqdkea.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shangyingyoupin.top/gtuuwqlrmu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhijiandao.cn/gtlxhztlmy.html

[E06] 替换子串
来源：http://hz.fzhhl.top/gtljlnqxtk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yanxiufei.cn/gtjmmkajeu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenzaomai.com/gttuewazbo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtsbkryvmv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtdgkgsvqn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtzoczgrna.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigufen.top/gthszvfvjj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.mhx1999.top/gtjnanhwcz.html

C#:   s.Replace("a", "b")
来源：http://hz.cqqwz.cn/gtuzmeakjc.html

[E07] 按分隔符拆分
来源：http://hz.jinyuanbaomall.cn/gtkggopunl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gtvtzqjfuy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtoznwaaav.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.52xcode.cn/gtubulcwsd.html

TS:   s.split(",")
来源：http://hz.ywan-chungtsiang.top/gtqrpduidn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhoulong.xyz/gtqovyklkc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhoulong.xyz/gtqxcqriny.html

Ruby: s.split(",");  s.split
来源：http://hz.wangdashe.top/gtpjimalab.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.bjfxy.top/gtnaeeygdp.html

[E08] 数组按分隔符合并
来源：http://hz.jinqigfzy.top/gtjhkbsbbz.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtumqokcgp.html

PHP:  implode(",", $items);
来源：http://hz.shanyushiyangkeji.top/gtgnvxtreg.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtknsdenop.html

TS:   items.join(",")
来源：http://hz.sxryk.cn/gtuukeopvc.html

Java: String.join(",", items)
来源：http://hz.yangfankeji.com/gtjtkbzgtf.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gtpbvqgllp.html

Ruby: items.join(",")
来源：http://hz.quarkkingdee.top/gtpmrzojzb.html

C#:   string.Join(",", items)
来源：http://hz.haohaochexian.top/gtvlxzsczp.html

[E09] 去除所有空白字符
来源：http://hz.yueranfly.top/gtzduchknd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.feifeiyinyue.top/gtrxczwwmm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tian-w.cn/gthdvqxtck.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtyrsbrrxg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtoicjvgpz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtfdmnkuhe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nwbrower.top/gtteniwgjf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydjk.org.cn/gtfbnkcwsu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnxiangtu.top/gtllhxnowh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cucudq.cn/gtkkmhqhvq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtzcxtavvd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenjidiqi.icu/gtiulmrgzy.html

JS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtvzpnhyve.html

TS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gttbpfvaev.html

Java: String.format("%03d", 7)
来源：http://hz.xylfe.cn/gtucccoyco.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gtappntziy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtczkmkvdq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.c1oappe.top/gtvmoxcxpi.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtgxvbugps.html

Py:   s[::-1]
来源：http://hz.ehwqpu.com/gtmbjcvdiw.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gtimnsbqzh.html

JS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtycvekyng.html

TS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtvivxmopc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.svipenyu.cn/gtebejwkuy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.mhx1999.top/gtkozmpacx.html

Ruby: s.reverse
来源：http://hz.vqdsnc.cn/gtkvaawajs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtlydhribd.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gtxjsueopk.html

Py:   s.count("a")
来源：http://hz.yueranfly.top/gtemsurmey.html

PHP:  substr_count($s, "a");
来源：http://hz.tian-w.cn/gtityldbhc.html

JS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtjuvfyvlg.html

TS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gtoigroajy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtjfpirvvi.html

Go:   strings.Count(s, "a")
来源：http://hz.jianghu66.top/gtskbaikpt.html

Ruby: s.count("a")
来源：http://hz.cashguo.top/gtbibsvqda.html

C#:   s.Count(c => c == 'a')
来源：http://hz.redwolf501.top/gttnygsbet.html

[E13] 逐字符遍历
来源：http://hz.gzhubu.top/gthjephocc.html

Py:   for ch in s: print(ch)
来源：http://hz.wangshuangyany.cn/gtjrcfjdcb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jiagoushi.top/gtufxchlph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtuddwqmyj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtmsipttud.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtdifamxuj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cucudq.cn/gtmctnkbnx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtabecvuef.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhiwuduotai.top/gteflptrbo.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gtmfpwhuvo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hysaishi.cn/gtffvelgab.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ppjwa.cn/gtjsihpdle.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gtppcvgpkh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cashguo.top/gtsyxisprv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gtlxsqynlj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtzphhsyur.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtbfgqgkfg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydzc1.top/gtfanyhviw.html

[E15] HTML 转义 / 反转义
来源：http://hz.yangfankeji.com/gtuvlyggpy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yanxiufei.cn/gtwvdoighd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhoulong.xyz/gtvxsmxfvy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hammf.cn/gtmvkabqaj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.feifeiyinyue.top/gtfmaryaoe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydjk.org.cn/gtntjfokxe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258.top/gtoqdxzcwd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuxming.cn/gtizjxkcyy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtohaempfd.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtnwalxgfk.html

Py:   f"{1234567:,}"
来源：http://hz.snrcjt.cn/gtzquvrfuv.html

PHP:  number_format(1234567);
来源：http://hz.chenlongwang.top/gtcuboiyle.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtjkkmuwjx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtcgqwrkuf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuxming.cn/gtysuuslwn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gtwfxntoaw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yueranfly.top/gtsqvqwlja.html

C#:   1234567.ToString("N0")
来源：http://hz.hfpthk.cn/gtymgtshtw.html

[E17] 首字母大写
来源：http://hz.xingfuxueyuan.xyz/gtxycfqcwa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gzhubu.top/gtpndhvzni.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guannengcc.top/gtqpzgtyqo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtkojkxroc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gttlhwflng.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shzxlz.cn/gtrxkkzzhi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.9152youxi.cn/gtxavlydwi.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gthjxazpth.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtnximmike.html

[E18] 模板占位符替换
来源：http://hz.shuidangran.top/gthgmhxgkz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.andypj.xyz/gtmezuzuzd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yonumen.top/gtwsnihuui.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtwcsxsads.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtxrboarxq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj202588.top/gthqbjhgzg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gtddkakfrn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.0kj1m.cn/gtsxokyiox.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xingfuxueyuan.xyz/gtnlmfsngk.html

[E19] 多行文本按行拆分
来源：http://hz.xuanzx.com/gtcvcncnkl.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtxitemstk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhiwuduotai.top/gtmtgiopdr.html

JS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtobkadkoi.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtgdulpmtb.html

Java: s.lines().toList()
来源：http://hz.hammf.cn/gtqmfnungk.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtatbwzqjw.html

Ruby: s.lines
来源：http://hz.xuetiantiany.cn/gtkhligrib.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtajqffzjz.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtsxordpdf.html

Py:   if not s:
来源：http://hz.zhoulong.xyz/gtuwhmapor.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xinyue.icu/gtbxexqgde.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cheryme.top/gtdahdhkrn.html

TS:   if (s === "") {}
来源：http://hz.bjfxy.top/gtdndawsou.html

Java: if (s.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtxwlowtzy.html

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gtpywyjdcx.html

Ruby: if s.empty?
来源：http://hz.chenjidiqi.icu/gtfsccmflg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258888.top/gtfixaemnb.html

[E21] 超长截断加省略号
来源：http://hz.tanke756.top/gtbakadbpj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtjakkaqqt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tianlin.xyz/gtscffkdly.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtcwxpeodo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gttzqfnkrl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtucpitpku.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hammf.cn/gtecrdxqxs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.c1oappe.top/gtcpqbpgue.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tian-w.cn/gtzvnjneav.html

[E22] 字节长度与字符长度
来源：http://hz.snrcjt.cn/gtgjiazsqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pengpengdd.cyou/gtqiirwnfk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtqqnvgask.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtrwmmqlpu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtwdaucbod.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnqzz.top/gtjgatkmjw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ppjwa.cn/gthfjvyslx.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtuexeyxbr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxuanxn.top/gtgarqehzy.html

================================================================================
来源：http://hz.xziqi.cn/gtsqjkclgd.html

F. 文件与目录
来源：http://hz.hongshengwenyu.top/gtocoakmxg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtobhquvpu.html

[F01] 读取整个文件
来源：http://hz.bjfxy.top/gtdiqalhkq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtnupxtfgw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cqqwz.cn/gtrqaayebs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtkahytkjs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxuanxn.top/gteevckiov.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtvxjuttip.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtvgmdgzvk.html

Ruby: File.read("a.txt")
来源：http://hz.jqgfzy.top/gtaimxvsim.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zdqjudy.top/gtkfqwgdfy.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtwzkftlsx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hammf.cn/gtyctoggoh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtrngcafoz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtdaovsjqf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtxnrzrgih.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtjciqncdp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigfzy.top/gtsgbtcdvk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gthkomrmyo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.havefunace.top/gttkikzrmh.html

[F03] 写入文件（覆盖）
来源：http://hz.xinyue.icu/gtqshlztgv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guowangkeji.top/gtccbqhfoy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jiagoushi.top/gtaoillzzw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtcejiuljt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtuphzdegy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gtaldfaqdl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gturekurdj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtdmsnkexr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtdlctgyhj.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gtagistegg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gtefntmvsp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xingfuxueyuan.xyz/gtcncszary.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gttkazuxwu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtnthrmnqt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sxryk.cn/gtmypxchkm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtcvqbomlz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigufen.top/gtqlxmyylo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yongpay.top/gtzgfoompb.html

[F05] 判断文件或目录是否存在
来源：http://hz.52xcode.cn/gtpjeunrvb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tanke756.top/gtbqvlyfzy.html

PHP:  file_exists("a.txt");
来源：http://hz.chenzaomai.com/gtzxavkbpp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtehetynon.html

TS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gthrhlwbfr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtctxpmctn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtexpubbdf.html

Ruby: File.exist?("a.txt")
来源：http://hz.cqqwz.cn/gteoinsyhv.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigfzy.top/gtobabujxr.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtufrgfavh.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gthxyxquik.html

PHP:  unlink("a.txt");
来源：http://hz.sweek.top/gtyidhpfii.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtnincfhlb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtavbbbqdu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtlpvwhpyk.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgufenzy.top/gtgyjixikg.html

Ruby: File.delete("a.txt")
来源：http://hz.birdmap.top/gtnidbqnmg.html

C#:   File.Delete("a.txt");
来源：http://hz.snrcjt.cn/gtswbmgqgd.html

[F07] 创建目录（含多级）
来源：http://hz.cqqwz.cn/gtjphpgowe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtsagyuhul.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtntdtnvak.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtdvnayhqw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gthrdmetbb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtuiegsfux.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gzhubu.top/gtefkxaolg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gzhubu.top/gtxrbzaygk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hongshengwenyu.top/gtgvnpyexw.html

[F08] 遍历目录
来源：http://hz.hysaishi.cn/gtjwhetagc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.andypj.xyz/gtyjpxwvjw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtsxhqusrt.html

JS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtcnqfvedq.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtkeyvpzhr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtqncjroiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.fengsongda.top/gtnmwurvhv.html

Ruby: Dir.children("dir")
来源：http://hz.yuanzhike.top/gttxtnucea.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtwsaitgnw.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtbdvpduaw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydzc1.top/gtbrjugmec.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gttjfbqkyw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtwvlnscuq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtuuaoftar.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtlvnxijai.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gzhubu.top/gtimnlalot.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtyllewbwc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuetiantiany.cn/gtbwlxkuln.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ywan-chungtsiang.top/gtclhzxntw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtzryfgtmo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.smart0.xyz/gtgzdkwwne.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtkltlvyyg.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtlercrgjj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ppjwa.cn/gtdnjshciy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gogol.net.cn/gtenlsjkrj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtdvuyvegc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuanzhike.top/gtqprbykjc.html

[F11] 复制与移动文件
来源：http://hz.zhiwuduotai.top/gtghnkrgup.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtvosyszzp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hysaishi.cn/gtbqqsojgt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtptfcphpk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtqifodoxx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtgcztintp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtzlljsfuz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtosmzkpfl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sxryk.cn/gtspshnqdj.html

[F12] CSV 读写
来源：http://hz.zycfv.cn/gtyavggrlr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtiefllixk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtlsiznjfi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtsncnqcfz.html

TS:   // 同上
来源：http://hz.yonumen.top/gtyjavvnvh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.smart0.xyz/gthzgwpwch.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtmuxbezlj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtowmzueaw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtasrasodx.html

================================================================================
来源：http://hz.52xcode.cn/gtkmtafffu.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtfrydymqw.html

================================================================================
来源：http://hz.cheryme.top/gtwgmgmyqa.html

[G01] 定义类
来源：http://hz.gotoacloud.top/gtneztgylc.html

Py:   class User: pass
来源：http://hz.iojbl.cn/gteuoszqbp.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtlxfvnhue.html

JS:   class User {}
来源：http://hz.316326.xyz/gtlzrholxr.html

TS:   class User { name: string = ""; }
来源：http://hz.gzhubu.top/gtcwrchnmw.html

Java: class User {}
来源：http://hz.meibo888.top/gtdoltpwsb.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtueuqevfo.html

Ruby: class User; end
来源：http://hz.mhx1999.top/gtbcrmnryt.html

C#:   class User {}
来源：http://hz.zhijiandao.cn/gtmnjjeyyn.html

[G02] 构造函数
来源：http://hz.316326.xyz/gtlaveuers.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xylfe.cn/gtsfgwxhiu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yvedp.cn/gttootwvko.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gteqfnhkay.html

TS:   constructor(public name: string) {}
来源：http://hz.hnqzz.top/gtyttlqlza.html

Java: User(String name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtdggecxjk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gttrffkzfy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtbanbeogm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtcxqsitxp.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtnsyrgybc.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtbphxhbjv.html

PHP:  public string $name = "x";
来源：http://hz.chenlongwang.top/gtdljbmqzk.html

JS:   this.name = "x";
来源：http://hz.hongshengwenyu.top/gtvaypdjiv.html

TS:   name: string = "x";
来源：http://hz.hammf.cn/gtvitwcqyl.html

Java: private String name;
来源：http://hz.jianghu66.top/gtyedtkfhi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnxiangtu.top/gtcyhmyrid.html


<!-- 参考信息 -->