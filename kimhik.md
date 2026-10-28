代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtxsnzvoke.html

Ruby: items.join(",")
来源：http://hz.jinghuilouyu.cn/gtlleefpue.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtlxdqkwxo.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtcdldsyfz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cdnleiting.top/gttbxzyxzt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtaigntmuu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yvedp.cn/gthkxninut.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtuerufqtw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtifmweikd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gtbuyjnnsc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gtqjwwxtmn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jyoumei.cn/gtaazpwtfp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dianchejie.cn/gtpscyqazb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gtcwfcvmef.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gttwrcozqr.html

JS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtxxmhvizp.html

TS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtllbiahel.html

Java: String.format("%03d", 7)
来源：http://hz.cucudq.cn/gtyxjzffri.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtycojnmua.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yvedp.cn/gtygfltobw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtlfqiwkzi.html

[E11] 反转字符串
来源：http://hz.gotoacloud.top/gtxjqppste.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gtdkzergwa.html

PHP:  strrev($s);
来源：http://hz.kuanghao11.cn/gtrjgrpald.html

JS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtpsaphgcg.html

TS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtxogkowzm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuetiantiany.cn/gtxodnidmi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tian-w.cn/gtpzlrygow.html

Ruby: s.reverse
来源：http://hz.zhixingplan.top/gtcmetmjua.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtzwusrtkv.html

[E12] 统计某字符出现次数
来源：http://hz.andypj.xyz/gtlkuhzplj.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtzfnlpdmg.html

PHP:  substr_count($s, "a");
来源：http://hz.zhoulong.xyz/gtsgoibsmb.html

JS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gtwpukquyn.html

TS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtgmvivcir.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jyoumei.cn/gtxbwqfdiu.html

Go:   strings.Count(s, "a")
来源：http://hz.xingfuxueyuan.xyz/gtoutkxcco.html

Ruby: s.count("a")
来源：http://hz.yuanzhike.top/gtpluczrpp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.smart0.xyz/gtprivmwgi.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtibdwgfbo.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtdmkdimrm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgfzy.top/gturjktevq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gttzcdlrlu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtnwheswqo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangshuangyany.cn/gtistcojgk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtbpsypfur.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtrrpvjelx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtbszmoyyo.html

[E14] URL 编码与 Base64
来源：http://hz.fzhhl.top/gtovlownwb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sufxvd.cn/gtobcezduo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gtkerphluu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jiagoushi.top/gthgtbxjsl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxuanxn.top/gtzqadvlub.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tanke756.top/gttqrtxnbu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hongshengwenyu.top/gtgixijukk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dianchejie.cn/gtsilnkozh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtusqfutvg.html

[E15] HTML 转义 / 反转义
来源：http://hz.shuidangran.top/gtswrwouri.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydzc1.top/gtkhhxdnag.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtuxkmtfzq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydjk.org.cn/gtdgmqdfme.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtczrurydz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gtxobzctpi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gtqkwfddjj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cashguo.top/gtexsydnkt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangshuangyany.cn/gtqtrgmxti.html

[E16] 数字千分位
来源：http://hz.jqgufenzy.top/gtuznoigvi.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtsjtakjer.html

PHP:  number_format(1234567);
来源：http://hz.wangdashe.top/gtbabqrdhi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtgljdczjk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtqbvcdlrb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258.top/gtlvvuwnfn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gttejseyks.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sweek.top/gtjhzjxmev.html

C#:   1234567.ToString("N0")
来源：http://hz.zhoulong.xyz/gttbezrlqa.html

[E17] 首字母大写
来源：http://hz.tianlin.xyz/gtvtnbalxo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhijiandao.cn/gtrovlylex.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jyoumei.cn/gtzlsbopbp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtdquzonhr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtmyqqyhic.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.meibo888.top/gttxeedghv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigufen.top/gtheujdgle.html

Ruby: s.capitalize
来源：http://hz.hnqzz.top/gtxcknkkga.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gtrhzduzgp.html

[E18] 模板占位符替换
来源：http://hz.jyoumei.cn/gthvnqilrv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinghuilouyu.cn/gtgmlbcvfl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gthidfskku.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtcjzrnvng.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtsjnjzyaz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xziqi.cn/gtubafijhc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtjuqzporw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.0kj1m.cn/gtzyimqopo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenlongwang.top/gtkimfluxw.html

[E19] 多行文本按行拆分
来源：http://hz.aibaodan.cn/gtoqrvufce.html

Py:   s.splitlines()
来源：http://hz.chenzaomai.com/gtbwwdxtms.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtxwurmjqu.html

JS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtykpcwbgv.html

TS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtjazmubfv.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtskjvoodh.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gtgqstxmpo.html

Ruby: s.lines
来源：http://hz.cqqwz.cn/gtbwntbzxi.html

C#:   s.Split('\n')
来源：http://hz.hnqzz.top/gtaaumkgmo.html

[E20] 判断字符串是否为空
来源：http://hz.cucudq.cn/gtpqzfndij.html

Py:   if not s:
来源：http://hz.jinqigufen.top/gtfzvzcfvr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtaqcyqtsn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jlsjyb.cn/gtletnyxck.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gtajaacnee.html

Java: if (s.isEmpty()) {}
来源：http://hz.tianlin.xyz/gttycgchlr.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtxgxamrmp.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gttpwtevfq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhaomingkeji.xyz/gtwehxpfzx.html

[E21] 超长截断加省略号
来源：http://hz.52xcode.cn/gtkxbhdswv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hongshengwenyu.top/gtvafyxynb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtczolfide.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gthaealvex.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtiwpmphvh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtasrggare.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gtsuwtpdxj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hywenlv.cn/gtisbfjgnh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenzaomai.com/gtlcxixdmw.html

[E22] 字节长度与字符长度
来源：http://hz.gotoacloud.top/gtownsmvhh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuanzx.com/gtwpuhsfwp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtqguqutpg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtdtbqftvf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gthahpvvmj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nwbrower.top/gteqnutakh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daria6918.cn/gthiibnhys.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhoulong.xyz/gtzamyzhgu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.smart0.xyz/gtrlhdlsgi.html

================================================================================
来源：http://hz.ybcxt.top/gthhxfyboj.html

F. 文件与目录
来源：http://hz.pengpengdd.cyou/gtbrriknzb.html

================================================================================
来源：http://hz.wangdashe.top/gtgijeamow.html

[F01] 读取整个文件
来源：http://hz.tianlin.xyz/gtcvcmtyfk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtxeuvvnfs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhengqikj.top/gtrviiuwmc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtlhdpnvya.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtqbspzqwa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sweek.top/gtlagdfjjg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxinkj.top/gtyzwgqupa.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtgsdpaiaw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gtxyjbzkzj.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtffraunqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aizwys.cn/gtpnkrumba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tianlin.xyz/gtvrpclrrt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtxhwxnupv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtyahcwmgz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtwdnaavqx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guowangkeji.top/gtojdzmlqn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pycfn.com/gtzfmaarhp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yongpay.top/gthzvfdtdx.html

[F03] 写入文件（覆盖）
来源：http://hz.zhongyouzk.top/gtjhseptok.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.iojbl.cn/gtpzvwiabk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gtddigyfjx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtcxzjcjjc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtrobxubkf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fengsongda.top/gtrjqiystx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ppjwa.cn/gtapgrbjey.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtjrldbgjb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gtphphaqld.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtsyxtjjqz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtykbahwzd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtzratxems.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtsxebffjd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhengqikj.top/gtfbsxsyri.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jianghu66.top/gtsbskiupd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhongyouzk.top/gtzccnfdak.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tianlin.xyz/gtyjdvsrch.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yvedp.cn/gtndardjuk.html

[F05] 判断文件或目录是否存在
来源：http://hz.jianghu66.top/gtqlelndbc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hammf.cn/gtbtppsgkq.html

PHP:  file_exists("a.txt");
来源：http://hz.yanxiufei.cn/gtvuafqnor.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtzocykapd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtrxweldya.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtnpahhyky.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jianghu66.top/gtnzphouea.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtelslwpkq.html

C#:   File.Exists("a.txt")
来源：http://hz.snrcjt.cn/gtvgllfryi.html

[F06] 删除文件
来源：http://hz.fengsongda.top/gthywaedcq.html

Py:   os.remove("a.txt")
来源：http://hz.gogol.net.cn/gtqbiijuky.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtpiolghyh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.316326.xyz/gticucqgeu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtivysgktb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtrbvtvnzo.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gtwfjqyhyz.html

Ruby: File.delete("a.txt")
来源：http://hz.yueranfly.top/gtjmvrznpt.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtzmvafvqd.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtrvbaaiby.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtqfpqcddj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtirncawin.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtmsyumhmo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtxxluxlwh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtzjnmsrhh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtudkaoqcz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtmfzmtolr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gtcdswozhz.html

[F08] 遍历目录
来源：http://hz.smart0.xyz/gtqhxklxqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhaomingkeji.xyz/gtsymkfija.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtjlyclmcg.html

JS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtgsblyiwv.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtwxjebjdb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtewdteers.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtviwsiywd.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gttnheeldj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daria6918.cn/gtcnuultbg.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gttactnwau.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ybcxt.top/gtbywironx.html

PHP:  filesize("a.txt");
来源：http://hz.dianchejie.cn/gtngjcdwtl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gttbpkmzfw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtdnfvjyyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtftvujykh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aibaodan.cn/gtzgdiazlu.html

Ruby: File.size("a.txt")
来源：http://hz.ydjk.org.cn/gtahlhldot.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zdqjudy.top/gttvghnbsh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gtwukjqgrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtdmkqulma.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gtjxaylneq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtykagunkm.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtxutlafyl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.mhx1999.top/gtgfbnmfdq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cdnleiting.top/gteddkabmd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtlgkitkwj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtbinsbcij.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtzxrbffmn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtddsvvgdb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtljlkxdsm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtitmbgywm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtrpqdzeso.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtobuosmbp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtrilsranw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtlgzgqwof.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dashuyun.cn/gtxptfjlwh.html

[F12] CSV 读写
来源：http://hz.iojbl.cn/gtnsgzliah.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gtlvazepnm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gtsawbmbeh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gttnpiowow.html

TS:   // 同上
来源：http://hz.0kj1m.cn/gtcnhsnlpw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtnsujizxg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ivvv.top/gtujjkfmmp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ppjwa.cn/gtzporxmtu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gtjnrcrgnr.html

================================================================================
来源：http://hz.52xcode.cn/gtboqwxyjj.html

G. 面向对象
来源：http://hz.daria6918.cn/gtectjgqpg.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtaikglxge.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtfvgawhud.html

Py:   class User: pass
来源：http://hz.jyoumei.cn/gtbzbovjng.html

PHP:  class User {}
来源：http://hz.bjfxy.top/gtqwdccjuo.html

JS:   class User {}
来源：http://hz.yj202588.top/gtxsthwghi.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gtulhaqnou.html

Java: class User {}
来源：http://hz.sysykeji.top/gtmljtzsbz.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtbdfpofjd.html

Ruby: class User; end
来源：http://hz.havefunace.top/gtsfnpxwyy.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtujkqyesv.html

[G02] 构造函数
来源：http://hz.hywenlv.cn/gtxbdyvmjk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtbkzqrfld.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cqqwz.cn/gtnodmegkj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtfrtqrjwr.html

TS:   constructor(public name: string) {}
来源：http://hz.gotoacloud.top/gtfndaweol.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydzc1.top/gtsxbrzzrr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtqksfowcq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtvgsncdja.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nwbrower.top/gthdrjoeix.html

[G03] 实例属性
来源：http://hz.pengpengdd.cyou/gtfcjabkca.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtnskcbvfw.html

PHP:  public string $name = "x";
来源：http://hz.nwbrower.top/gtfvkpaqxf.html

JS:   this.name = "x";
来源：http://hz.bjfxy.top/gtqdjofhjj.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtthjwicxo.html

Java: private String name;
来源：http://hz.yj202588.top/gtztjorjlo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zycfv.cn/gtwzoetooj.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtiarjrlts.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aibaodan.cn/gtenaigrjj.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gthagxkcjr.html

Py:   def greet(self): return self.name
来源：http://hz.hywenlv.cn/gtkvsbivci.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtvthyygdf.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtcoftfjnb.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtnudvncah.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtrrbtlhef.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.haohaochexian.top/gtrtqtzhhf.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtozwviycp.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gttwariqfx.html

[G05] 继承
来源：http://hz.smart0.xyz/gtfmqwstkn.html

Py:   class Admin(User): pass
来源：http://hz.xingfuxueyuan.xyz/gtishacdqp.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtfjequaii.html

JS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtziqzrilf.html

TS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtzteytpns.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtdnhrkkgs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xingfuxueyuan.xyz/gtuphelorg.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtslntqsow.html

C#:   class Admin : User {}
来源：http://hz.pengpengdd.cyou/gtsyljmdax.html

[G06] 重写方法
来源：http://hz.shzxlz.cn/gtynmwqyyx.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gthajdaigk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtzvvnpuyq.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtgurokesm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtttiedgxw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtwmlobeur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hywenlv.cn/gtlczfefqt.html

Ruby: def greet; "admin"; end
来源：http://hz.ivvv.top/gtztkxijgi.html

C#:   public override string Greet() => "admin";
来源：http://hz.meibo888.top/gtwdubqlho.html

[G07] 调用父类方法
来源：http://hz.tian-w.cn/gtewxggcss.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtvpbpaflc.html

PHP:  parent::greet();
来源：http://hz.ybcxt.top/gtxoiisujg.html


<!-- 参考信息 -->