代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nwbrower.top/gtfqtfogtf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gthkakmhkb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtdfoekoik.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xziqi.cn/gtsjbatqbl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gtmovhybxh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ywan-chungtsiang.top/gttjgocyzz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jianghu66.top/gtrsjvlpwx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.smart0.xyz/gtcsnelwjv.html

[E06] 替换子串
来源：http://hz.shanyushiyangkeji.top/gttpeabktt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtcbqhjqna.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenzaomai.com/gtooxgpvnu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtrtiwdvld.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtkwionzxx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtfijrigpc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xziqi.cn/gtulmdbnsh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtvblwnrnj.html

C#:   s.Replace("a", "b")
来源：http://hz.tian-w.cn/gtztkdedef.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtngxbicaa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.vqdsnc.cn/gtxznqpztr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gtzduhoctm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.kuanghao11.cn/gttzcxyceq.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gtrtbakiyp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ybcxt.top/gtgibmgzqz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gthojgxxjx.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtvzkxobon.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ehwqpu.com/gtysqbfhhk.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtznjyejup.html

Py:   ",".join(items)
来源：http://hz.meibo888.top/gtwijndxvp.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtqcfbmwat.html

JS:   items.join(",")
来源：http://hz.cqqwz.cn/gtaasarrpa.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtxkjjmkmy.html

Java: String.join(",", items)
来源：http://hz.chenlongwang.top/gtgvawxdtc.html

Go:   strings.Join(items, ",")
来源：http://hz.zhijiandao.cn/gtiognhoxe.html

Ruby: items.join(",")
来源：http://hz.jyoumei.cn/gtcukxdafb.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gtctutuxab.html

[E09] 去除所有空白字符
来源：http://hz.zhengqikj.top/gtpfljwpwx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.fzhhl.top/gtjildcifv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xziqi.cn/gtgldlvslt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtwbujhwtk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtbfrcebdt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigufen.top/gtuquikgqe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fengsongda.top/gtjznqgjpe.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhixingplan.top/gtxxhlvkyg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shuidangran.top/gtnhivlrzi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.9152youxi.cn/gtqtmcotkx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtrdhujual.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhaomingkeji.xyz/gtqcdymlaf.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtpfwwneok.html

TS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtmfglseye.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtmjcfvwva.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydzc1.top/gtrloispoy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtoxydzetr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zdqjudy.top/gtxnfdbztg.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtjzzzrbxj.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtdldjdwse.html

PHP:  strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtcqnkyuwg.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gturwakdvk.html

TS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtovzcoubn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gogol.net.cn/gtvlvipukt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sweek.top/gtnxlazkzq.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gtaswlokxx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtosfgguof.html

[E12] 统计某字符出现次数
来源：http://hz.wangdashe.top/gtkzxjlsvq.html

Py:   s.count("a")
来源：http://hz.snrcjt.cn/gtweyyrerw.html

PHP:  substr_count($s, "a");
来源：http://hz.birdmap.top/gtlpfemaqq.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtcrtnclia.html

TS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gtdnvcddxp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aibaodan.cn/gtmalhhkqx.html

Go:   strings.Count(s, "a")
来源：http://hz.xuetiantiany.cn/gtoolrpokp.html

Ruby: s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtubdezfek.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tianlin.xyz/gttzfvucpz.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gtkxacnlmt.html

Py:   for ch in s: print(ch)
来源：http://hz.daria6918.cn/gtksenakoh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtiqnigbqk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtbytibgtv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gthmywiwof.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtjldvovaq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pycfn.com/gtjdtpamsf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.snrcjt.cn/gtdpacqgxn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ehwqpu.com/gtwxltfmdk.html

[E14] URL 编码与 Base64
来源：http://hz.chenjidiqi.icu/gtjdewprmd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtwkearxiw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cheryme.top/gtimbdjfcp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tianlin.xyz/gthhnzmhzm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dianchejie.cn/gtnhdjjnqo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sysykeji.top/gtaqodapzp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydzc1.top/gtqkgjdtos.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtegevyctl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.andypj.xyz/gteoxqlmbq.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtttcdyevz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtjhqhllkx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinghuilouyu.cn/gtejisyfun.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtmlmmujfi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sufxvd.cn/gtazrwthtd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtslyikepc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigufen.top/gtbaijxwzu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tanke756.top/gtjxelbmvd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenjidiqi.icu/gtiqlxkyzi.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gteobnnfhd.html

Py:   f"{1234567:,}"
来源：http://hz.gzhubu.top/gtxvaxbgeq.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtdudjtbkr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtrkyaapcr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gthyqfhmth.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shzxlz.cn/gtsykikojj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guannengcc.top/gtftortvnp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gthdqmiqvh.html

C#:   1234567.ToString("N0")
来源：http://hz.xylfe.cn/gtnsrkhtjx.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtyhdlnxts.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sysykeji.top/gtuxatqxsx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtacfzkwwx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtkuhzdgfu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gthmoebhib.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gttttowsew.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cqqwz.cn/gtownpgzgp.html

Ruby: s.capitalize
来源：http://hz.jiagoushi.top/gtwjsefrbx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cdnleiting.top/gtcuettoxp.html

[E18] 模板占位符替换
来源：http://hz.zhaomingkeji.xyz/gtmbiccozq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jlsjyb.cn/gtqntojwlv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gtrtkgdadn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtejfumxzl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtrhpsfnrm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ppjwa.cn/gtloqfwund.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gtbzeghdqr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtpzskhehc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ywan-chungtsiang.top/gtkbrgdxgz.html

[E19] 多行文本按行拆分
来源：http://hz.birdmap.top/gtxbvodtef.html

Py:   s.splitlines()
来源：http://hz.yanxiufei.cn/gtswympece.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gtltvshicm.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtenxgzsje.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtaejvyexj.html

Java: s.lines().toList()
来源：http://hz.xuetiantiany.cn/gtohzaqunr.html

Go:   strings.Split(s, "\n")
来源：http://hz.zycfv.cn/gtfnyadcjq.html

Ruby: s.lines
来源：http://hz.zhiwuduotai.top/gtdnkfdfej.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtywqjqiio.html

[E20] 判断字符串是否为空
来源：http://hz.wangshuangyany.cn/gtjrklvnlt.html

Py:   if not s:
来源：http://hz.0kj1m.cn/gthpvqjxkn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtiitnqwco.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtcjkkkwet.html

TS:   if (s === "") {}
来源：http://hz.sweek.top/gtnwrqquzo.html

Java: if (s.isEmpty()) {}
来源：http://hz.316326.xyz/gtmratmztm.html

Go:   if s == "" {}
来源：http://hz.dianchejie.cn/gtdyxxmied.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtywqkeoas.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gzhubu.top/gtkfbbhsce.html

[E21] 超长截断加省略号
来源：http://hz.ivvv.top/gtabzijuem.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtgaajpftl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.haohaochexian.top/gtjzjzrhho.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtvkfkuptl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gttjmkunlt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtybbwirvi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guowangkeji.top/gttjdmbsho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cucudq.cn/gtprmnzlxy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.52xcode.cn/gtpfalxcvo.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtjicutzzo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinyuanbaomall.cn/gtybpvppzx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtbxdlvqri.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtskwhkjnx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtxsypygog.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xylfe.cn/gtzqdfrqbo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtdelizklv.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxuanxn.top/gtuvixchev.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.fengsongda.top/gtottapavl.html

================================================================================
来源：http://hz.xuanzx.com/gtyqzzljqg.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtjnjgrwnh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtknxizxmg.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gtdkbyswgw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtrzuolutz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhongyouzk.top/gtxldtoppk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgfzy.top/gtcaznjfdk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtaqkgnten.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtqzlaynrx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dianchejie.cn/gtueuqkrof.html

Ruby: File.read("a.txt")
来源：http://hz.xziqi.cn/gtkfueslhu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gtpskyhcvb.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gterklkdoj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gogol.net.cn/gthvtrxpul.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yonumen.top/gtzvxfctvw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gttqjhqvtt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtywkjaufk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtcpwpqjmf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gtwswymfki.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gzhubu.top/gteilnkjtd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gtjyckwzot.html

[F03] 写入文件（覆盖）
来源：http://hz.chenlongwang.top/gteoghmwgg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtahtqmrny.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtwypqzxnf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtxhapcmzs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtwlqskeup.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtekyoujmb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtegjgtjhe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yueranfly.top/gtbfkteipr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtqworsxpq.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtuoztyutr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtcldcvrkc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtjmpgwuqb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtkihcbpaq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtjqoknyas.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxinkj.top/gtcjpzonki.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtihvozqfw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shuidangran.top/gtiuorunux.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.9152youxi.cn/gtmbaxxxbe.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtlyteodog.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtwlmhfskt.html

PHP:  file_exists("a.txt");
来源：http://hz.ydzc1.top/gtekcvzgja.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtushtrrpv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxafrtbvq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtiuyornun.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.svipenyu.cn/gtugaxqfcv.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtdbcwuuya.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtisqdbonb.html

[F06] 删除文件
来源：http://hz.xuanzx.com/gtjobksasi.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtofivxbwq.html

PHP:  unlink("a.txt");
来源：http://hz.hysaishi.cn/gtrvoumykw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtehigwtqu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtjeiajsyq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtlvglmkoc.html

Go:   os.Remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtdslkchov.html

Ruby: File.delete("a.txt")
来源：http://hz.tian-w.cn/gtgqbizpvn.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gteuvhwxhn.html

[F07] 创建目录（含多级）
来源：http://hz.zhiwuduotai.top/gtyxtahkwh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ehwqpu.com/gtrjvqrisu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhaomingkeji.xyz/gtrrmalgyu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtgawtichi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gthxsqvrqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhiwuduotai.top/gtqyyuqdfe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xingfuxueyuan.xyz/gtvqavwzty.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.c1oappe.top/gtlwgktaoj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gzhubu.top/gtzsfckzzx.html

[F08] 遍历目录
来源：http://hz.yangfankeji.com/gtsszqcoyp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtumhixamg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtvafhgckr.html

JS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtbqexlruw.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtcdfdtuih.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtvzfendgb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.kuanghao11.cn/gtvnrzpmjk.html

Ruby: Dir.children("dir")
来源：http://hz.jyoumei.cn/gtokplxnxm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cqqwz.cn/gtxonwcphc.html

[F09] 获取文件大小
来源：http://hz.guannengcc.top/gtciviuuib.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daria6918.cn/gtdhcehchz.html

PHP:  filesize("a.txt");
来源：http://hz.zycfv.cn/gtpnjbasvd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fzhhl.top/gtzuockzny.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtvlnyvxaz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtesujvbmd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gzhubu.top/gtpdpwxkkn.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtbkukdyps.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtflqoreqd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gthpltelmm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtzsgemdih.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtssfqngwy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtliqbntjc.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtbprlbxdn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.mhx1999.top/gtwwonvscp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtdkmavrpj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtarvwdemj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtvkknqlzd.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangtech.top/gtdspgfljt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtmhfqknoj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtycvjfxom.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gttodsakjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtndbwgweg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.c1oappe.top/gtmdcsblcf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.bjfxy.top/gtkmibbula.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtwhadfobr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tianlin.xyz/gtparbjtgh.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtqeucbanj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.smart0.xyz/gtogztrfis.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gtmzxyngtu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtiwsunzpz.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gtivfndmbl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gthvfcslox.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pengpengdd.cyou/gtfoyqunrt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj202588.top/gtbnbajqdr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.birdmap.top/gttvoicwcq.html

================================================================================
来源：http://hz.nwbrower.top/gtajkccggw.html

G. 面向对象
来源：http://hz.jianghu66.top/gtuqdeuxww.html

================================================================================
来源：http://hz.guannengcc.top/gtxlrocolu.html

[G01] 定义类
来源：http://hz.pengpengdd.cyou/gtwbcszfsp.html

Py:   class User: pass
来源：http://hz.ydjk.org.cn/gtoctpwzrc.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gteymrgykg.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtjekugdeq.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtbkiymnjq.html

Java: class User {}
来源：http://hz.mhx1999.top/gtivgwndho.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtgwecpqbm.html

Ruby: class User; end
来源：http://hz.yanxiufei.cn/gtqjzgourk.html

C#:   class User {}
来源：http://hz.zycfv.cn/gtxoakytqh.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtesjlqzdg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gtrjtupogx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtfhbhkdqd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtgndhllxx.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtyiufycqk.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtciomwxtg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtsgokflzf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gtpseypjqo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xziqi.cn/gtymuqykik.html

[G03] 实例属性
来源：http://hz.zycfv.cn/gtljfgfrtw.html

Py:   self.name = "x"
来源：http://hz.haohaochexian.top/gtzskdcdnh.html

PHP:  public string $name = "x";
来源：http://hz.hywenlv.cn/gtvnvdalph.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gtcieqhclm.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gteitmyttd.html

Java: private String name;
来源：http://hz.hnqzz.top/gtowxyhtoo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zdqjudy.top/gtiuibktby.html


<!-- 参考信息 -->