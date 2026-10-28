代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtarwgxmrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtrozhrwax.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sweek.top/gtqsbzgyyn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jianghu66.top/gtieiqvppv.html

C#:   s.Replace("a", "b")
来源：http://hz.mhx1999.top/gtklprzviu.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtaskhchgy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinghuilouyu.cn/gtjwtxirly.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuanzhike.top/gtzmjzmrng.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhixingplan.top/gtijubmcpp.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtfiygplni.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gzhubu.top/gtyumambpo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xziqi.cn/gtjcpitxke.html

Ruby: s.split(",");  s.split
来源：http://hz.sysykeji.top/gtcdkjihmw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gotoacloud.top/gtouqlayom.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtbphgigny.html

Py:   ",".join(items)
来源：http://hz.ehwqpu.com/gtdqfemvcn.html

PHP:  implode(",", $items);
来源：http://hz.jqgfzy.top/gtaartkcma.html

JS:   items.join(",")
来源：http://hz.jyoumei.cn/gtataxlumm.html

TS:   items.join(",")
来源：http://hz.ivvv.top/gtjuwmwrkq.html

Java: String.join(",", items)
来源：http://hz.haohaochexian.top/gtfgsbtofj.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gtvhtzdkyv.html

Ruby: items.join(",")
来源：http://hz.iojbl.cn/gtvwiounnm.html

C#:   string.Join(",", items)
来源：http://hz.gzhubu.top/gtdawildsn.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtcykvkulm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtmeufvgvi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yueranfly.top/gtwreuocuv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtjhbqtetu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gticbkrbxi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aizwys.cn/gthrpivsew.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.9152youxi.cn/gtcehoocmz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.snrcjt.cn/gtxukuoacz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangdashe.top/gtbpskkbpt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenjidiqi.icu/gtusohoays.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.feifeiyinyue.top/gtkewycsct.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nwbrower.top/gtzugxuhml.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtqlouijiw.html

TS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtxkhzlbtx.html

Java: String.format("%03d", 7)
来源：http://hz.cucudq.cn/gtlykcrtjn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtabpqqyhk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.snrcjt.cn/gttxzvtvlj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.feifeiyinyue.top/gtjlzttojh.html

[E11] 反转字符串
来源：http://hz.yuanzhike.top/gthbpbcfgh.html

Py:   s[::-1]
来源：http://hz.zycfv.cn/gthopjjjnp.html

PHP:  strrev($s);
来源：http://hz.ppjwa.cn/gtsaehseam.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtorvhuetm.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gthuuqfzyh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gtedzlkugz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtzbqkzdpp.html

Ruby: s.reverse
来源：http://hz.hnxiangtu.top/gtalglzdyw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtfffjguzt.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtjwkaspqf.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtlvxhciaf.html

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gtpzcnagyz.html

JS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtjhamyljq.html

TS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtzcbathvs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtulrvafsr.html

Go:   strings.Count(s, "a")
来源：http://hz.ydjk.org.cn/gtdwucsknp.html

Ruby: s.count("a")
来源：http://hz.fengsongda.top/gtqtffcmrm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhoulong.xyz/gtdrxniqgk.html

[E13] 逐字符遍历
来源：http://hz.dianchejie.cn/gteoptrvwx.html

Py:   for ch in s: print(ch)
来源：http://hz.wangshuangyany.cn/gtesdqjwmt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj202588.top/gtjomigzcc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtimwoxdxk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtgjwqvheh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtonwahmfg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtiyuyphyv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aizwys.cn/gtbpxmdzjc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.quarkkingdee.top/gtzdhwfhqo.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gtkxkcacqj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.wangshuangyany.cn/gtalfcdrfe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ppjwa.cn/gtbhnqwoai.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtgesrtqxj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtzyjccxoq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gtlkwohngr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.svipenyu.cn/gtunygrovr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.9152youxi.cn/gtszjnganq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj202588.top/gtgmgntjtp.html

[E15] HTML 转义 / 反转义
来源：http://hz.pycfn.com/gtxjoqfqna.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sysykeji.top/gtauavxfut.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinghuilouyu.cn/gtjovvyeil.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtnhkayadp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtsjntbeet.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.smart0.xyz/gtvpswfqgl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.feifeiyinyue.top/gtdqalgaxt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sxryk.cn/gtxfeiyvgk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigfzy.top/gtpzbxsner.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtblimalox.html

Py:   f"{1234567:,}"
来源：http://hz.jiagoushi.top/gtynjwxtqi.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtpinxlfsk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtnxtlgyci.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gttfgmqgxd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ppjwa.cn/gtlfwaxkzi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sweek.top/gthsdrdywq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aibaodan.cn/gtdpapuvrj.html

C#:   1234567.ToString("N0")
来源：http://hz.ywan-chungtsiang.top/gtvrsoxjun.html

[E17] 首字母大写
来源：http://hz.yvedp.cn/gtllljpbka.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.meibo888.top/gtibratoak.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cheryme.top/gtorhvflvu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtjqiifydo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtvixlhfye.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtxeujoqfy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtukztuxta.html

Ruby: s.capitalize
来源：http://hz.sufxvd.cn/gtkzskriil.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hammf.cn/gtjeksrvif.html

[E18] 模板占位符替换
来源：http://hz.tianlin.xyz/gtiacxnhbb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daxiang520.top/gthlytufde.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuanzhike.top/gtqfghhbcz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtwazkjyrs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtxelflzax.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gthwxgypfj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnxiangtu.top/gtygrhvcti.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zdqjudy.top/gtqjfaszcw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zycfv.cn/gtpgrrjbdg.html

[E19] 多行文本按行拆分
来源：http://hz.yanxiufei.cn/gtcygsdypc.html

Py:   s.splitlines()
来源：http://hz.sysykeji.top/gtavoyjlgo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtyuhcrybg.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtevfuoktf.html

TS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtlogyirdk.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtuaffwlkn.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinqigufen.top/gtonwjosld.html

Ruby: s.lines
来源：http://hz.316326.xyz/gtdddyzezs.html

C#:   s.Split('\n')
来源：http://hz.zhoulong.xyz/gteqdvmqpa.html

[E20] 判断字符串是否为空
来源：http://hz.jiagoushi.top/gtmgjzaerh.html

Py:   if not s:
来源：http://hz.ybcxt.top/gttdqucdvj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnxiangtu.top/gtswevjwgd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangtech.top/gtepynqfyc.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtdijspmlt.html

Java: if (s.isEmpty()) {}
来源：http://hz.sysykeji.top/gtpxkkllux.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtwqmcuzfg.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtuzloyzid.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ywan-chungtsiang.top/gtbzolakrg.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtzvnqkuwh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.kuanghao11.cn/gtukvwwcaa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tanke756.top/gtlosuktci.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtqtvblcir.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtektqtbfw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtcskhxljm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtumtmztte.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.smart0.xyz/gtchyxpklg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zycfv.cn/gtygzrsfis.html

[E22] 字节长度与字符长度
来源：http://hz.yvedp.cn/gtdhrcedkb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gtsklpiewf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtskuzdehw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtjnxyymha.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cdnleiting.top/gtemyietzk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shangyingyoupin.top/gtmpcexnsz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtxqeiipka.html

Ruby: s.bytesize;  s.length
来源：http://hz.jyoumei.cn/gtzixandfk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtsfydqhlu.html

================================================================================
来源：http://hz.shuidangran.top/gtdphpnzix.html

F. 文件与目录
来源：http://hz.52xcode.cn/gtljpbqukm.html

================================================================================
来源：http://hz.tian-w.cn/gtmdbtsvlm.html

[F01] 读取整个文件
来源：http://hz.316326.xyz/gtznjyprsn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtudepzkmd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtnudgocdq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnxiangtu.top/gtlnwcrzht.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtcdbltuyk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtcpzwivvj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtncmccjbi.html

Ruby: File.read("a.txt")
来源：http://hz.gotoacloud.top/gtqlluelze.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtzkiyaylb.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtxpqgcvad.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gttccgpekv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtoawttvdu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtngqofgbg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtowjcfymi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gtiaktmngs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ppjwa.cn/gtseqtvxfs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtlyxbjxli.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shangyingyoupin.top/gtbpmadzza.html

[F03] 写入文件（覆盖）
来源：http://hz.birdmap.top/gtgocankcz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ehwqpu.com/gtvvafxqbp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gtlvmyohhv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtfhlkoorb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtpyjieoyz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sxryk.cn/gthklnqarw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yuxming.cn/gtxuphjrco.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.52xcode.cn/gtrctrpwhy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtmjlyyasi.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gtymvzxioh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtbmhflcdm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtazdvbdfi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtbhtmjhvt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtkraprvfi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtfepsasfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangkeji.top/gtqgyavtli.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yonumen.top/gtvlzicdgq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydzc1.top/gtbvbdrscs.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gttahldfmq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuxming.cn/gtpxndtzwt.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtitmpzeca.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtqctnpabv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtkbrproak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtyvncwecg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtruymazew.html

Ruby: File.exist?("a.txt")
来源：http://hz.dianchejie.cn/gtbsyjqctd.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtsuomnmyx.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtyjqfuzsv.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtjlnyzptf.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gtzjomqhsm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtdslzvjlm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtjgyeowtx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gticgtbjya.html

Go:   os.Remove("a.txt")
来源：http://hz.aizwys.cn/gtwrtejpvv.html

Ruby: File.delete("a.txt")
来源：http://hz.iojbl.cn/gtyjtyphnn.html

C#:   File.Delete("a.txt");
来源：http://hz.feifeiyinyue.top/gtprioreuv.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtoueynfjt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gtmadlsjpi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenzaomai.com/gtcodkgdqj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtxwxaqmde.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtinctvyri.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtbegcjdkz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtizawozvt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xingfuxueyuan.xyz/gtwyehwtyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hywenlv.cn/gtndpmxrrv.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtdhunsxhl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hysaishi.cn/gtlgvepabi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gtxzcbkokz.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangtech.top/gtrtgpqehs.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gteqhosunr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtvhdsivdc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tian-w.cn/gtplfofdwk.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gtgddmtszh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cucudq.cn/gtpwsrllhj.html

[F09] 获取文件大小
来源：http://hz.yanxiufei.cn/gtsopplyoi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.pengpengdd.cyou/gtljkoxslo.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtmfcudseq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtyimpmuxl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtosebpqek.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtnsecmbbu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtufcouwik.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtfxtqizzm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtzvbavukw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.mhx1999.top/gtjrbrwrmk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gthxwnwuzf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shzxlz.cn/gtbdgogmlk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtiyrucfdi.html

TS:   path.extname("a.txt")
来源：http://hz.52xcode.cn/gtofnccewx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.snrcjt.cn/gterritfpx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtksnfokoi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gteukfofld.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gzhubu.top/gtlscmguxg.html

[F11] 复制与移动文件
来源：http://hz.zdqjudy.top/gtjksmmprq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtguqovlqd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.andypj.xyz/gtcnfcwehl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtagsppwao.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtjohbhkfs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aizwys.cn/gtjzhveoad.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gthtndifev.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtqwhahjxm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yueranfly.top/gtfcigikqj.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtfhxcoudh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gttvpyekxc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258.top/gtrctqtmzu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sweek.top/gtuyvhilia.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtkkkoizmj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtjrmrkxkp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtytcqvyow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtmdyzughn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhengqikj.top/gtxgbvncqd.html

================================================================================
来源：http://hz.pengpengdd.cyou/gteeiavvhm.html

G. 面向对象
来源：http://hz.zhijiandao.cn/gtafcartrv.html

================================================================================
来源：http://hz.ybcxt.top/gtmqevfwbd.html

[G01] 定义类
来源：http://hz.cucudq.cn/gthyujgabl.html

Py:   class User: pass
来源：http://hz.yangfankeji.com/gtvvutkqoz.html

PHP:  class User {}
来源：http://hz.yj202588.top/gtqxckwphx.html

JS:   class User {}
来源：http://hz.yj20258.top/gtpbpybveu.html

TS:   class User { name: string = ""; }
来源：http://hz.jinyuanbaomall.cn/gtqwgpbfnm.html

Java: class User {}
来源：http://hz.nanxinkj.top/gtquyznqfm.html

Go:   type User struct { Name string }
来源：http://hz.jinyuanbaomall.cn/gtiubedcig.html

Ruby: class User; end
来源：http://hz.xuanzx.com/gtipzkegpi.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtyvhkytde.html

[G02] 构造函数
来源：http://hz.redwolf501.top/gtitrjakks.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pycfn.com/gttupkgyry.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hysaishi.cn/gtxksapsds.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtjikifqrr.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtcjhbpuuj.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtmpwkcizc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guannengcc.top/gtkmmmqhbp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.vqdsnc.cn/gtolvaxvmy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gtxvfyjlvc.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gtabpypwio.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtklgkbpnv.html

PHP:  public string $name = "x";
来源：http://hz.andypj.xyz/gtrcwpjyoo.html

JS:   this.name = "x";
来源：http://hz.yonumen.top/gtfxfpzxno.html

TS:   name: string = "x";
来源：http://hz.xziqi.cn/gtlptnsmue.html

Java: private String name;
来源：http://hz.jiagoushi.top/gtfcpxefnx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuanzhike.top/gtqtlyuxok.html

Ruby: @name = "x"
来源：http://hz.jinqigfzy.top/gtihqwlats.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtdsorifnd.html

[G04] 定义方法
来源：http://hz.iojbl.cn/gthxuypruc.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtdjdqhmex.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtmxrmiipm.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtocgbmoyo.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtvcvhjkuw.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtrusuhihn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtkerqpvrg.html

Ruby: def greet; @name; end
来源：http://hz.havefunace.top/gtukgebjcv.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtojvvbtvc.html

[G05] 继承
来源：http://hz.feifeiyinyue.top/gtqdqilhji.html


<!-- 参考信息 -->