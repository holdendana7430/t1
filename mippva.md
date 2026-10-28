代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.yj202588.top/gtyqrihqqw.html

Ruby: items.join(",")
来源：http://hz.yangfankeji.com/gtsukrodak.html

C#:   string.Join(",", items)
来源：http://hz.yj202588.top/gthncgskjs.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtggfehhqw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xylfe.cn/gtfwfjboei.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtgciqwiqg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtvyjximkz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtpzvympem.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuetiantiany.cn/gtlyqdmhwv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sysykeji.top/gtzcvdrqcj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tanke756.top/gtxofzkqec.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenzaomai.com/gttcivanyv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yueranfly.top/gtajgnskrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtrhkyherd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhiwuduotai.top/gtsddivacn.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtcaijpyaj.html

TS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtgrynedoz.html

Java: String.format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtmgrjndvh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cucudq.cn/gtlahkvwhy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hammf.cn/gtjmnjvwyv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.birdmap.top/gtoviimvax.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtmpndczoj.html

Py:   s[::-1]
来源：http://hz.aizwys.cn/gtujcnehai.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtirfqutfq.html

JS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtlucdhgic.html

TS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtqppyhntx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jyoumei.cn/gtngkrlmhd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtqualtonv.html

Ruby: s.reverse
来源：http://hz.zdqjudy.top/gtmzceebrp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtfgygksbq.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gtnzkkthhl.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtulzacwgy.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtqrghaiaf.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtuepadzwq.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtfmtmsuqr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gtdabyuhht.html

Go:   strings.Count(s, "a")
来源：http://hz.sweek.top/gtkvdiplmx.html

Ruby: s.count("a")
来源：http://hz.ybcxt.top/gtyzgzekln.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gtwzdljmtu.html

[E13] 逐字符遍历
来源：http://hz.yuanzhike.top/gtslzvapmz.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gtatupnggt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigufen.top/gtsdecppyj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhiwuduotai.top/gtrykruubl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtbhosnezb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daxiang520.top/gtsytollxc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.snrcjt.cn/gtmriutwae.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.birdmap.top/gtfxahhyxu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuanzx.com/gtxxwklger.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtkrijposq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sweek.top/gtekgwlnbb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.mhx1999.top/gtniyoohwc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtnxxlzbcw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.bjfxy.top/gtwlsexbus.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtlwqrleov.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.mhx1999.top/gtjuwrqfmp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtwdxjelsp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gzhubu.top/gtgmvkbrqx.html

[E15] HTML 转义 / 反转义
来源：http://hz.cqqwz.cn/gtekowlwmo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gtsfwdflds.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinghuilouyu.cn/gtksfolhkn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.haohaochexian.top/gtrqxqhuaf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydzc1.top/gtaabkseol.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.snrcjt.cn/gtiexgukmu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fengsongda.top/gtzofmobbz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dianchejie.cn/gtwgvcbxbn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gteejadhei.html

[E16] 数字千分位
来源：http://hz.zhijiandao.cn/gtoictnpuh.html

Py:   f"{1234567:,}"
来源：http://hz.hnxiangtu.top/gtukowvxnd.html

PHP:  number_format(1234567);
来源：http://hz.0kj1m.cn/gtjpspazek.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gtadywatpr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtwguwzked.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtuasftjac.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cheryme.top/gtyijzbgrx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxuanxn.top/gtqffjepoc.html

C#:   1234567.ToString("N0")
来源：http://hz.ydzc1.top/gtajyrpexi.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gtbezatzjh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuxming.cn/gtzklrmgly.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hysaishi.cn/gthcowfjxn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtuvytmmju.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtafbwiftx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gzhubu.top/gthnuhlwjf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gogol.net.cn/gtgsattexx.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtfndhvuju.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtjgmrapwu.html

[E18] 模板占位符替换
来源：http://hz.sxryk.cn/gteoyphsfa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xziqi.cn/gtuockvlod.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yonumen.top/gtxfcnkbys.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtuvvpheop.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gthzbpogkr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.svipenyu.cn/gtmbaavehz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtzvcjxwdf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxinkj.top/gttcrjyunp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fzhhl.top/gtsqzaiwgm.html

[E19] 多行文本按行拆分
来源：http://hz.chenlongwang.top/gtnywfbeta.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangkeji.top/gtimjyggik.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtgxquecul.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtmsxrvpkt.html

TS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gtksjxphkc.html

Java: s.lines().toList()
来源：http://hz.zycfv.cn/gtztydzrfv.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gtxuualvkx.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtxcpnizne.html

C#:   s.Split('\n')
来源：http://hz.0kj1m.cn/gtjriktbir.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtqeqitlot.html

Py:   if not s:
来源：http://hz.pengpengdd.cyou/gtrpxshnpr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ppjwa.cn/gtzavieraq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xziqi.cn/gtkbaqtdoq.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtzuwyskou.html

Java: if (s.isEmpty()) {}
来源：http://hz.xziqi.cn/gtgrjtonko.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gtmytoqtcr.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtmzvxizkl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yanxiufei.cn/gtzbqrwuzm.html

[E21] 超长截断加省略号
来源：http://hz.fengsongda.top/gtruyjpzjc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xingfuxueyuan.xyz/gtrgbjuvyc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aizwys.cn/gtjfhhidbk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtbsrcxhpl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtsmncibox.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtnwktsjmu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.0kj1m.cn/gtufubwkjr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gtdnwdsnwr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guannengcc.top/gtcypzjrub.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gttfxtcnmj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.birdmap.top/gtufmfwttk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtqztkuxek.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtsofmgvig.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtltjhkxhp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gotoacloud.top/gtrxldrqqf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fzhhl.top/gtnamqdnso.html

Ruby: s.bytesize;  s.length
来源：http://hz.tanke756.top/gtsgwmlsjp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aibaodan.cn/gtfwmoezto.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkrfnqvqb.html

F. 文件与目录
来源：http://hz.cdnleiting.top/gtfyuevyla.html

================================================================================
来源：http://hz.kuanghao11.cn/gtiimevcne.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtjbaytuby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.9152youxi.cn/gtpgthcvny.html

PHP:  file_get_contents("a.txt");
来源：http://hz.andypj.xyz/gteanmihnp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aizwys.cn/gtjsixceln.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dashuyun.cn/gtmkgdttsw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtdnlelwop.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtveoaypaw.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gtfoglrqxd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtpiwolvpi.html

[F02] 逐行读取文件
来源：http://hz.ehwqpu.com/gtgtdxiqtx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.smart0.xyz/gtgvshmbsu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sxryk.cn/gtgmykilck.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gtquksytrn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtghypxzbz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tanke756.top/gthekifmtx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gticxixprd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xinyue.icu/gtlypwyyoz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pycfn.com/gtmsdhxdpt.html

[F03] 写入文件（覆盖）
来源：http://hz.iojbl.cn/gtybowzvcf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gtphtlnqtq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtrvfheuyr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtkskwvues.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtocsurjzc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cucudq.cn/gtpevhqxod.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtphxpfpil.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.snrcjt.cn/gtpmkwjbrw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtczearttb.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtqhpcypje.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenlongwang.top/gtzhjoktfs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuanzhike.top/gtuoblnzkw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cucudq.cn/gtgszgcrsi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gthvuffbix.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sweek.top/gtvagntavj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtisxcclsw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtfollwuwi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangtech.top/gtlckloltp.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigfzy.top/gthgllijrl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhixingplan.top/gtqmjikhyc.html

PHP:  file_exists("a.txt");
来源：http://hz.xinyue.icu/gtxqotxetd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtbdxqpyjp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtzlqglmiw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtgswncyhy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dianchejie.cn/gtltlpwnho.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gtlxfzzojz.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtjigqmzly.html

[F06] 删除文件
来源：http://hz.gaohongyu789.top/gtqzgietkd.html

Py:   os.remove("a.txt")
来源：http://hz.gzhubu.top/gthputxtbj.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtajbnzldd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtzzotzldt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtcwoccfgq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtfssvzefl.html

Go:   os.Remove("a.txt")
来源：http://hz.sufxvd.cn/gtiapfroch.html

Ruby: File.delete("a.txt")
来源：http://hz.shzxlz.cn/gtnzoliwtc.html

C#:   File.Delete("a.txt");
来源：http://hz.316326.xyz/gtulsdokdm.html

[F07] 创建目录（含多级）
来源：http://hz.andypj.xyz/gtznjinzth.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtvalmbbrn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangdashe.top/gtgjqkwnhk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gttzzilmyc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtegvkklqv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhijiandao.cn/gtosvzwawp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtpghcdtyp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtxhedscuh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shzxlz.cn/gtdzsjxtwt.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtdjibgqkk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangtech.top/gtawbntavh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtwiruluof.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtlyozhmgq.html

TS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtfvvbwten.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gttsttuhwp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.316326.xyz/gtapvpirlw.html

Ruby: Dir.children("dir")
来源：http://hz.nwbrower.top/gtrwwbmtuc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hongshengwenyu.top/gtnpjheyxg.html

[F09] 获取文件大小
来源：http://hz.ywan-chungtsiang.top/gtkhwdopsx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daria6918.cn/gttxdhqldz.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtaceiyvnq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtrittkmur.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtbqqshbll.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtnetcfhdf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgfzy.top/gtrsutxjqr.html

Ruby: File.size("a.txt")
来源：http://hz.jiagoushi.top/gtvezemjyu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cashguo.top/gteqyrouff.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jlsjyb.cn/gtijeuywzb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtqpwuaqna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gaohongyu789.top/gtxzfcbzwx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtocaaznfe.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangkeji.top/gttsdeiage.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fengsongda.top/gtnaglvxia.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daria6918.cn/gtnfroznjz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtgmktbdpq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtxpqgtheb.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangkeji.top/gtlrpgrrjk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtzedqrdfz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtgvhmbsuo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtbphfewdi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtcwjanzwi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.haohaochexian.top/gtwxzewbds.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cqqwz.cn/gtppvfakxx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtvmcdrwww.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtnimnuutq.html

[F12] CSV 读写
来源：http://hz.shanyushiyangtech.top/gtqlcyijfs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258888.top/gtyfadwcss.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.snrcjt.cn/gtuactubfb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.havefunace.top/gtcztxndcs.html

TS:   // 同上
来源：http://hz.hnxiangtu.top/gtkqsjhuef.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gtdmnjxily.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtbsthqfqw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gzhubu.top/gtvhddrnir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yvedp.cn/gtylrnuvqu.html

================================================================================
来源：http://hz.sufxvd.cn/gtykghgxca.html

G. 面向对象
来源：http://hz.aizwys.cn/gtzleadein.html

================================================================================
来源：http://hz.meibo888.top/gtmyiidplg.html

[G01] 定义类
来源：http://hz.9152youxi.cn/gthnenmvhd.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtvycsopgy.html

PHP:  class User {}
来源：http://hz.9152youxi.cn/gtewgiqfya.html

JS:   class User {}
来源：http://hz.cheryme.top/gtsvzctnfh.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtqvyjsltk.html

Java: class User {}
来源：http://hz.xingfuxueyuan.xyz/gttytzgzpv.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gthdfbhuug.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gtllqymzoq.html

C#:   class User {}
来源：http://hz.snrcjt.cn/gtrrtpmcfx.html

[G02] 构造函数
来源：http://hz.dianchejie.cn/gtiyiguzzc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gtsqzrhysn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtcmslvlju.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aizwys.cn/gtfcowtijc.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtaxuowgrd.html

Java: User(String name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtnzgfolmr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.0kj1m.cn/gtjphbmqki.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtmjhcicza.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aizwys.cn/gttargxxjn.html

[G03] 实例属性
来源：http://hz.pycfn.com/gtaiciwdmx.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtlrdhxecb.html

PHP:  public string $name = "x";
来源：http://hz.316326.xyz/gtrdpeazhq.html

JS:   this.name = "x";
来源：http://hz.guannengcc.top/gtppeurmsf.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtisgykxhf.html

Java: private String name;
来源：http://hz.xuetiantiany.cn/gtitdgvltr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtzcybmgpm.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtkalovxky.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigufen.top/gtqpswzaow.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtboleqfhk.html

Py:   def greet(self): return self.name
来源：http://hz.0kj1m.cn/gtxcbojcna.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtpoaydijb.html

JS:   greet() { return this.name; }
来源：http://hz.fengsongda.top/gtlazmrutj.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtewgibuqb.html

Java: String greet() { return name; }
来源：http://hz.xylfe.cn/gtrectwpce.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtmkidgypv.html

Ruby: def greet; @name; end
来源：http://hz.gzhubu.top/gtzqwmpgle.html

C#:   public string Greet() => Name;
来源：http://hz.pycfn.com/gtxppfamui.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtxatohkbt.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtlzqobavr.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gtlhkoouoa.html

JS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gteummxupp.html

TS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtffzttige.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtbbimamwr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenlongwang.top/gtfumycbet.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtnicvobnd.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtgrgywehr.html

[G06] 重写方法
来源：http://hz.cashguo.top/gtbiwsiozi.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtinboavtb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtpjcyygjb.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtjevkyzbe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtnpnjxdvb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daria6918.cn/gthwvjtsal.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gaohongyu789.top/gtncpdjkxv.html

Ruby: def greet; "admin"; end
来源：http://hz.tianlin.xyz/gtgwkqhqan.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtzajslbxq.html

[G07] 调用父类方法
来源：http://hz.hfpthk.cn/gtiechtfxj.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtahazvvcj.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtyusdxfhf.html


<!-- 参考信息 -->