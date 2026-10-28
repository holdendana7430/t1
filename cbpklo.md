代发 wailian999

[E06] 替换子串
来源：http://hz.pycfn.com/gtafngodug.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.meibo888.top/gtgwaebete.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.c1oappe.top/gttlaonxli.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtlzxhqtos.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtbwpfoxiy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtrfjgxlbt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hammf.cn/gtfxudeklw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yvedp.cn/gtonwybsup.html

C#:   s.Replace("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtketyuvck.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gtiwriqalq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtzyghojrz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenzaomai.com/gtvrkxewga.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sysykeji.top/gtzdwmqxww.html

TS:   s.split(",")
来源：http://hz.ywan-chungtsiang.top/gtmmwxzkfa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ppjwa.cn/gtqusoyokt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtqoivvwiw.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gtnhpfxzqp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydzc1.top/gtzcesrrfo.html

[E08] 数组按分隔符合并
来源：http://hz.redwolf501.top/gtpmjdqqnu.html

Py:   ",".join(items)
来源：http://hz.jinghuilouyu.cn/gtwratkdjz.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gtlkrudsbd.html

JS:   items.join(",")
来源：http://hz.nanxinkj.top/gtptshsccr.html

TS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtusqsggwa.html

Java: String.join(",", items)
来源：http://hz.xuanzx.com/gtvvzbagec.html

Go:   strings.Join(items, ",")
来源：http://hz.fengsongda.top/gtkzqeftho.html

Ruby: items.join(",")
来源：http://hz.cucudq.cn/gtsthdiuao.html

C#:   string.Join(",", items)
来源：http://hz.jinqigufen.top/gtgfaeiwyu.html

[E09] 去除所有空白字符
来源：http://hz.guowangkeji.top/gtesthusjx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ehwqpu.com/gtdaoewheb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yvedp.cn/gtrbdlpshg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtybrejtad.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gthtzpxabe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigufen.top/gtdenahfaw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtdrjdrryy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xylfe.cn/gtzblubhjn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtrolbvqcx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ybcxt.top/gttshoyxnc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjfxy.top/gtaejwmlmk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.meibo888.top/gtllymmoye.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtbpnsxztp.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtsafulljv.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtzahyctcy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cdnleiting.top/gtqkmwkaae.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gtlvtozhcy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.mhx1999.top/gtwxpiowlp.html

[E11] 反转字符串
来源：http://hz.pengpengdd.cyou/gtdvdxfwkm.html

Py:   s[::-1]
来源：http://hz.zhengqikj.top/gtpdppjxwu.html

PHP:  strrev($s);
来源：http://hz.hfpthk.cn/gtnucektul.html

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtcrkkqjhn.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtayxpdmxe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtqttxqwqx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.havefunace.top/gtqqtlqkjz.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gtjvzdumjv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtnjhrqirt.html

[E12] 统计某字符出现次数
来源：http://hz.xingfuxueyuan.xyz/gtknlkuuhj.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gttcgidulk.html

PHP:  substr_count($s, "a");
来源：http://hz.dianchejie.cn/gtcdasgiwk.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtrpjfuuiv.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangkeji.top/gtknjsgvls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtgmhypasp.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtrkcpbryk.html

Ruby: s.count("a")
来源：http://hz.zhoulong.xyz/gtzaowaqpt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gogol.net.cn/gtlqxikuie.html

[E13] 逐字符遍历
来源：http://hz.52xcode.cn/gtaxfmzuik.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gtpicpjfne.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.9152youxi.cn/gtosgnhpeu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtrkpbirgb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtaapitkfk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtpotrcztg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sweek.top/gtsburqjps.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fengsongda.top/gtblyngsuw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gzhubu.top/gttjfcaueu.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtyqfjicui.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gzhubu.top/gtnidrfcfs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gtvjsoklqp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yueranfly.top/gtgqtahggd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhoulong.xyz/gtrxkqssxy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zdqjudy.top/gtlleducvu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtfkxrrkkj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgufenzy.top/gtcidriwwp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhiwuduotai.top/gtzeyjpuwx.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtzpekhrut.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtfnvwpdvf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daria6918.cn/gtawpbymub.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gtttehmtyj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hysaishi.cn/gtwolzsgcx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yvedp.cn/gtrnkzdxjs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtjliboekm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tanke756.top/gtqeonhndg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnxiangtu.top/gtkzlrsauv.html

[E16] 数字千分位
来源：http://hz.jinqigfzy.top/gtpmyesixi.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gttoreaccu.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtdjtjfmhw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtifocnyhp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtkuurcszx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nwbrower.top/gtdbrxwpsm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jianghu66.top/gtehuweibb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258.top/gtdagjrcnb.html

C#:   1234567.ToString("N0")
来源：http://hz.fengsongda.top/gttvpxpqnw.html

[E17] 首字母大写
来源：http://hz.yongpay.top/gtvgcfoqiz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cheryme.top/gtclijxnlr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jiagoushi.top/gtsjwejkmm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gttwgafocy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtaskbwdjt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtnzwfuagw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.havefunace.top/gteeiwtkhj.html

Ruby: s.capitalize
来源：http://hz.vqdsnc.cn/gtivwbduxo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yueranfly.top/gtedualgso.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gtootkxrrq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtvumfnjih.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tianlin.xyz/gtcpjjviwe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtlzqgoybz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtduxggfrm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ybcxt.top/gtlvnankgc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtzzfubpdy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtbzryifii.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yongpay.top/gtgumhapyv.html

[E19] 多行文本按行拆分
来源：http://hz.xingfuxueyuan.xyz/gtgyfynfia.html

Py:   s.splitlines()
来源：http://hz.316326.xyz/gtzioigilf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtzxwqvyvu.html

JS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtwuqbdwmu.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtgvkluyan.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtqnzicxcx.html

Go:   strings.Split(s, "\n")
来源：http://hz.haohaochexian.top/gtamqcviio.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtovwxynna.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gtsuvokmey.html

[E20] 判断字符串是否为空
来源：http://hz.tian-w.cn/gtbbphsmpa.html

Py:   if not s:
来源：http://hz.zdqjudy.top/gtidtluhks.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtdbtaqyzb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtiidhhrmq.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtjbdtvxla.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtrwwvsmab.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtlzvzcglu.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gtlylkvwqm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gtanbudmwk.html

[E21] 超长截断加省略号
来源：http://hz.hnxiangtu.top/gtqftaabgb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtpxhpatgu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtiepasron.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtcwuxikzd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtirrhaghp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtmioqrjds.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtboysjmvt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gttlhqyonw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fengsongda.top/gtmboqnawi.html

[E22] 字节长度与字符长度
来源：http://hz.jiagoushi.top/gtoaautesz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gttfagxfns.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtfxmxyrey.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtafclxzeg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtjvscfdlk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnqzz.top/gtcdvswtsg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gaohongyu789.top/gtxonqhtlj.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtuulzjcvx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hywenlv.cn/gtzylsyvju.html

================================================================================
来源：http://hz.hysaishi.cn/gtmnpxpjce.html

F. 文件与目录
来源：http://hz.ivvv.top/gtpzqyqvqa.html

================================================================================
来源：http://hz.yvedp.cn/gtjafgpfiw.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gtqzqpzrtk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtodhtcokf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yueranfly.top/gtheqnpyib.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtxtkacyop.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gtrwggltbx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtqhyqivfg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.andypj.xyz/gtwukqcaaq.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtfdypzyvf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.0kj1m.cn/gtymummrjg.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtfodlblno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gogol.net.cn/gtwjtljprh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtgbxltpgu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gthwbnzmzf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtsmfqqpdd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtltosamyy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jlsjyb.cn/gttkwekolv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenlongwang.top/gtmkodicrt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigfzy.top/gtrolxccyw.html

[F03] 写入文件（覆盖）
来源：http://hz.yuanzhike.top/gtekvuduav.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinyuanbaomall.cn/gtgjmvxmcz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gteumzbxtk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sxryk.cn/gtwzwswtdk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtbtogpzqx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gttfpkohyn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtfqdeorln.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fzhhl.top/gtzkvqgarx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtjlwmcazq.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtozirduma.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gttiekposg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cheryme.top/gtddlkltdh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtohjbvbpp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gthuqyatel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtzxapxjho.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtwiiwgejc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtgxegyjup.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.daria6918.cn/gtjosgewgv.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtvmqzzvai.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gttdaidllc.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gtwaslragb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtipezzfqf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtyabnvqrt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtfpntwdiz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gttoqnhlla.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gtligdkaea.html

C#:   File.Exists("a.txt")
来源：http://hz.sysykeji.top/gtnfpzzabi.html

[F06] 删除文件
来源：http://hz.sweek.top/gtqchxfine.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtdmjbercu.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gtsoserbot.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtptoatvsw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtkjrjwzfk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtneovlyhn.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtcwihcptv.html

Ruby: File.delete("a.txt")
来源：http://hz.cqqwz.cn/gtombqwubm.html

C#:   File.Delete("a.txt");
来源：http://hz.jinghuilouyu.cn/gtpanfqxbz.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gttegzdzdd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gogol.net.cn/gtisodtest.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258888.top/gtqrowtljk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtfzkkcxpi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtbylorzrv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtlobyacmx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gtteaufiqn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.0kj1m.cn/gtwoyheocy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.snrcjt.cn/gtywrkemun.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtukskvbcz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shuidangran.top/gtdqjjydcf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtzxttyyfl.html

JS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtqkbkclhr.html

TS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gthfyndwqy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtvqvbqptd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtpeynwlhc.html

Ruby: Dir.children("dir")
来源：http://hz.yvedp.cn/gtxgqknnnk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gttkhpucxa.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtdmsudupu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yueranfly.top/gtwfejozqp.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtieyilryb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gtgssiibdw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtixqeyity.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtswfmccqp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtxfutbsow.html

Ruby: File.size("a.txt")
来源：http://hz.zhijiandao.cn/gtqvcozudt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtbelipgbv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtucihjojc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtwhxxdtpt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zycfv.cn/gtarjkibtw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gteikattju.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gtxanqslik.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gtbqoyxmfv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtxdzeutgo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtgrhlzpat.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtjufswcbx.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtkuxhddbk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtmozhxuzz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.iojbl.cn/gtbaacshzq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtsgyifjrw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtfqllbtiz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtzverqdtt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gtbpjmkxez.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtysuomwau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.aibaodan.cn/gtjjslondt.html

[F12] CSV 读写
来源：http://hz.yongpay.top/gtfgiurdif.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuxming.cn/gtrkhrfnem.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtewnnvjur.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhijiandao.cn/gtnnejgrbr.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtenegatzy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtsihuutgl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gthxqrazrs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnxiangtu.top/gtuwwzvosu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gthteggrjl.html

================================================================================
来源：http://hz.9152youxi.cn/gttxqsydhp.html

G. 面向对象
来源：http://hz.meibo888.top/gtxddgdbrn.html

================================================================================
来源：http://hz.sysykeji.top/gtdisgqubb.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtnpbangmt.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtgavynkof.html

PHP:  class User {}
来源：http://hz.ywan-chungtsiang.top/gtnyetxwzt.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtpclopuqg.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtazmkfnak.html

Java: class User {}
来源：http://hz.tanke756.top/gtzgmexfru.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtjkjlouob.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtvrjzdmtq.html

C#:   class User {}
来源：http://hz.shangyingyoupin.top/gtvilmbduk.html

[G02] 构造函数
来源：http://hz.guannengcc.top/gtolmyfmke.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtflmjsonk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtvasmmmui.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtfqunjjwy.html

TS:   constructor(public name: string) {}
来源：http://hz.0kj1m.cn/gtksuzzfck.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuxming.cn/gtqelthuls.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtzxqanuid.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtkgfjajfj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtqxqzksur.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtdgiiweur.html

Py:   self.name = "x"
来源：http://hz.jianghu66.top/gtorbysogz.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtbjfpwncc.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtuirwwpwr.html

TS:   name: string = "x";
来源：http://hz.gaohongyu789.top/gttybhcxnm.html

Java: private String name;
来源：http://hz.sysykeji.top/gtoubhgoay.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guowangkeji.top/gtlefhsysh.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtzpvjxgmm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtonwccikb.html

[G04] 定义方法
来源：http://hz.tianlin.xyz/gtypmvmebx.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtlsryrhxt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtntbieltv.html

JS:   greet() { return this.name; }
来源：http://hz.hfpthk.cn/gtfjtktqfv.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtpohhyrst.html

Java: String greet() { return name; }
来源：http://hz.hysaishi.cn/gtflphtnil.html


<!-- 参考信息 -->