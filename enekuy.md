代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtlnfddzpt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenzaomai.com/gttggdybrp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gttfdjxwdc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtkwtdyjml.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangtech.top/gtdddgkwln.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ywan-chungtsiang.top/gtpeigvgwa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zycfv.cn/gtlhbeaati.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nwbrower.top/gtkujoadlu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtxsizfvag.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtpkucxmso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dashuyun.cn/gtifvopwyl.html

JS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtfakiamtl.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtvbptipmj.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtdynctmiv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtwvipqqft.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtgfpehyje.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtkxhutlyd.html

[E11] 反转字符串
来源：http://hz.sxryk.cn/gttdzsxovl.html

Py:   s[::-1]
来源：http://hz.quarkkingdee.top/gttfuxjrag.html

PHP:  strrev($s);
来源：http://hz.0kj1m.cn/gtvaovgaub.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtpprqhyhh.html

TS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtqmdupyob.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuanzhike.top/gtmybxyzpa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtjzroihrg.html

Ruby: s.reverse
来源：http://hz.sxryk.cn/gteabbfbka.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtefaqdigc.html

[E12] 统计某字符出现次数
来源：http://hz.meibo888.top/gtqcqaypbx.html

Py:   s.count("a")
来源：http://hz.9152youxi.cn/gtacywwjeb.html

PHP:  substr_count($s, "a");
来源：http://hz.ydzc1.top/gtonjdrhyq.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtxoxkwbmt.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtgknqwizh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gthfueuzan.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtotdanzfz.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtsipqgkwn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xziqi.cn/gthzjfzpmg.html

[E13] 逐字符遍历
来源：http://hz.ywan-chungtsiang.top/gtgpyacyfh.html

Py:   for ch in s: print(ch)
来源：http://hz.jlsjyb.cn/gtqemwhykl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gaohongyu789.top/gtmzgjlbep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtjemrjfgb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtlxjaxnes.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtqrwzksmb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhaomingkeji.xyz/gtgmtzwcbz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gtmvvfvqjg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnxiangtu.top/gtwpddolra.html

[E14] URL 编码与 Base64
来源：http://hz.ybcxt.top/gtpgihtuar.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgufenzy.top/gtlosccbvp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jiagoushi.top/gtmfacfgpw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.feifeiyinyue.top/gtimidvtjg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gtjswivpjw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtyaegqefz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtscieulnj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenjidiqi.icu/gtewtxstla.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtxurwtrxp.html

[E15] HTML 转义 / 反转义
来源：http://hz.fzhhl.top/gthbqrdmfs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhoulong.xyz/gtuycmsnwn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.9152youxi.cn/gtrytuuxvs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.wangshuangyany.cn/gtkpggbcqq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuanzhike.top/gterjprdmv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydzc1.top/gtyvyxjdgi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnxiangtu.top/gtynpxfcku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtbjwgeuxf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fengsongda.top/gtybrvojuj.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtldyzafyz.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigufen.top/gtqyngmprf.html

PHP:  number_format(1234567);
来源：http://hz.wangdashe.top/gtimpexxxb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtoyvkfxip.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtghiepdgv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tianlin.xyz/gthskunzny.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.svipenyu.cn/gtfkplqmyy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sxryk.cn/gtsxorlwmb.html

C#:   1234567.ToString("N0")
来源：http://hz.jinghuilouyu.cn/gtcydasoef.html

[E17] 首字母大写
来源：http://hz.hfpthk.cn/gtqwbxticd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xinyue.icu/gtqjbmbfjw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtwrovrkzj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtltfvacad.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gteqdmmaar.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hysaishi.cn/gtymnwaqar.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tian-w.cn/gtxzuwazel.html

Ruby: s.capitalize
来源：http://hz.yj202588.top/gtcjwakjkf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtsvcmuzjq.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtbgfdhgtv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.kuanghao11.cn/gtftwensaf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jianghu66.top/gtwxlxjjxs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtldkjpycc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtkiudydzn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtjsrfuque.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtpuhgazyu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtzyilyysj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtuxalurvq.html

[E19] 多行文本按行拆分
来源：http://hz.snrcjt.cn/gtkgvlwjgn.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gtxpwoclij.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuetiantiany.cn/gtsryhhujh.html

JS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtcrwaavyu.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtarkuadqf.html

Java: s.lines().toList()
来源：http://hz.aibaodan.cn/gtanweutwx.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydjk.org.cn/gtqmuyuxba.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtpfyubhuw.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gthargqzqd.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtekjwpcpc.html

Py:   if not s:
来源：http://hz.birdmap.top/gtzegyvyfw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yangfankeji.com/gtwwnmfovu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.bjfxy.top/gtiivyiifb.html

TS:   if (s === "") {}
来源：http://hz.sxryk.cn/gtiqbcbwff.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtmzwsqsta.html

Go:   if s == "" {}
来源：http://hz.zhaomingkeji.xyz/gtlzvmbzam.html

Ruby: if s.empty?
来源：http://hz.yuxming.cn/gtuuipsclr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gtiirlghnb.html

[E21] 超长截断加省略号
来源：http://hz.daria6918.cn/gtxqrazlth.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gtzmrbiywx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtjgxgrbba.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtzzflvebp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtqbkczvxz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtcfaccizu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shuidangran.top/gtshozzxcu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.mhx1999.top/gtalepnpew.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtucmtmvpp.html

[E22] 字节长度与字符长度
来源：http://hz.yonumen.top/gtftdxoywa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yangfankeji.com/gtvgmqbqxr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtyonvgwpj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtzkpndxgt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtifyemakf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtruacqhhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtizwtijte.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtpygxzhhn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jlsjyb.cn/gtdwkpkkxt.html

================================================================================
来源：http://hz.jiagoushi.top/gtacckfogs.html

F. 文件与目录
来源：http://hz.yongpay.top/gtywnpmcwb.html

================================================================================
来源：http://hz.xinyue.icu/gtzcdhghdn.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtytutavqn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtacriooad.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtrhquacid.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gttjmlvugy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pycfn.com/gtsgdohmxx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtvbwaegwq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuanzx.com/gtghtkihse.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtpeeyqkkt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtlzuxonvd.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gtjksoalpk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigfzy.top/gtvikqmzuw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shangyingyoupin.top/gtvmtxglwc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtsyekrdrx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtjmnwhpvr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtmijqoxcd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtnbydshkl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhaomingkeji.xyz/gtvmrzgtyg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhijiandao.cn/gtktjteuhx.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gtebwgjfac.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ppjwa.cn/gtzjtciurz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtakwgccie.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gthcbjwwrh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtvttnufpv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgfzy.top/gtkfoshibd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yueranfly.top/gtcltxecpp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ybcxt.top/gtdfxaspjm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yongpay.top/gteduiqoia.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtietekswe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aibaodan.cn/gtdbftpvkm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtjmtsafup.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtaivansad.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtpbnkeulo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgfzy.top/gtvizmmcpt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gttznrsqfi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhixingplan.top/gtbxighjua.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.316326.xyz/gtxdrlgdwl.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gtsidqrugm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtxundmmum.html

PHP:  file_exists("a.txt");
来源：http://hz.xziqi.cn/gtoioyxwgg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtgcyjcwyk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtgmcmjevk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtlwalwgnk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtwqpubcaq.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuxming.cn/gtlswskzav.html

C#:   File.Exists("a.txt")
来源：http://hz.xylfe.cn/gtqjpwnyfk.html

[F06] 删除文件
来源：http://hz.316326.xyz/gttpaytpra.html

Py:   os.remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtvkdoxsjt.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gthazzkwik.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtpdjrzhfb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtgmslhspp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtmrvbiout.html

Go:   os.Remove("a.txt")
来源：http://hz.sxryk.cn/gtqknrpuhw.html

Ruby: File.delete("a.txt")
来源：http://hz.xuetiantiany.cn/gtpejcrlrr.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtgfwuezgc.html

[F07] 创建目录（含多级）
来源：http://hz.redwolf501.top/gtzeefmhfn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuxming.cn/gtjvkdmouj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hammf.cn/gtsfrdlnpk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtwtdghvzd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtpnbgpsic.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtyroyvzao.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guowangkeji.top/gtegzgfkvl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgufenzy.top/gtqfaivrha.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtuvxpcjfv.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gtcfzolidt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtiipqxvjw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydjk.org.cn/gtbdxbhkuh.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtcgdxvbmo.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtprhtgwoa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtostxbpqz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhixingplan.top/gtsqqwgkjy.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gthwumqwvy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtuqcqxfcy.html

[F09] 获取文件大小
来源：http://hz.yj202588.top/gtscsyprrw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gtnnogtirn.html

PHP:  filesize("a.txt");
来源：http://hz.quarkkingdee.top/gtjvfccopa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtjsbithea.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtigjnchgh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtcoppbujq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.iojbl.cn/gtbyprlrym.html

Ruby: File.size("a.txt")
来源：http://hz.fzhhl.top/gtlmtowqeb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jyoumei.cn/gtzjzbkhph.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtcussmvjy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtibsncaba.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shangyingyoupin.top/gtuotmnoky.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtpjlgints.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtpbycfkdc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtousmeagv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sysykeji.top/gtieyznlcj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtaqrisnoq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gttwewcovr.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangtech.top/gtepfanoon.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtoblmxgyo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aizwys.cn/gtqoratbvn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtyjkfsawm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtljtswipw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gtemgvsitp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shuidangran.top/gtpkoatgmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gttodvzhxw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.meibo888.top/gtcoznoqcz.html

[F12] CSV 读写
来源：http://hz.xziqi.cn/gtdhattvai.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gtkouhfueu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.birdmap.top/gtzohcesjc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fzhhl.top/gtxmbarkzv.html

TS:   // 同上
来源：http://hz.redwolf501.top/gtrnussrje.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhixingplan.top/gtafkhrppv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jlsjyb.cn/gtrvpebvfm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenjidiqi.icu/gthutafiuk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.bjfxy.top/gtmlzwcqee.html

================================================================================
来源：http://hz.ivvv.top/gtljjovdjo.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtljfczhwd.html

================================================================================
来源：http://hz.aibaodan.cn/gtpghpqmgx.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtjsbjptpj.html

Py:   class User: pass
来源：http://hz.dashuyun.cn/gtkbeslsgs.html

PHP:  class User {}
来源：http://hz.gotoacloud.top/gtmltrhzuj.html

JS:   class User {}
来源：http://hz.ppjwa.cn/gtdjxxumvl.html

TS:   class User { name: string = ""; }
来源：http://hz.gotoacloud.top/gtceelzptl.html

Java: class User {}
来源：http://hz.meibo888.top/gtxkowkeop.html

Go:   type User struct { Name string }
来源：http://hz.shzxlz.cn/gtcjryjxpr.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtbcqfqvgj.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtofdovisp.html

[G02] 构造函数
来源：http://hz.yangfankeji.com/gthpzgzseu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtbcltlltr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtfoeajner.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hammf.cn/gthixkwfpv.html

TS:   constructor(public name: string) {}
来源：http://hz.yongpay.top/gtlxeibcyr.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtmvspeazh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj202588.top/gtawjskqkr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gtwxgqkynn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenzaomai.com/gtlgtoudbd.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtnvwzyqmr.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtqgtnxbdy.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtlykhxhpj.html

JS:   this.name = "x";
来源：http://hz.xuanzx.com/gtolpfoxze.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtbmqtrcmi.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gtwfyoizso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangkeji.top/gtwnxbawhv.html

Ruby: @name = "x"
来源：http://hz.zhaomingkeji.xyz/gtlnlpdqer.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtgxjejoow.html

[G04] 定义方法
来源：http://hz.iojbl.cn/gtzczsngoq.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtgppzlxgy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtuiqccati.html

JS:   greet() { return this.name; }
来源：http://hz.sweek.top/gtmxfrkkum.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtjmwacdfd.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangtech.top/gtvwdvozll.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtmhbgprld.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtxnyhykna.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtpkhrxvfb.html

[G05] 继承
来源：http://hz.sweek.top/gtglacrmqo.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtghcuuqky.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtckawvyxb.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtxjrupmjl.html

TS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gthjkbqtnh.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtfqkhtwti.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtlmbjxdve.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangkeji.top/gtfxpqstkq.html

C#:   class Admin : User {}
来源：http://hz.sweek.top/gtarcdccbq.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gtmsrrplcq.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gtauclfzwx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gthdcqplji.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtnqzjlane.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtvdrwwcux.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtsclzcdly.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yanxiufei.cn/gtwdguubic.html

Ruby: def greet; "admin"; end
来源：http://hz.yuanzhike.top/gtkazhtvcz.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtfoysokpl.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtfpxhqask.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtmnftxdzk.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtxfkfyfdn.html

JS:   super.greet();
来源：http://hz.birdmap.top/gthsllxikz.html

TS:   super.greet();
来源：http://hz.pycfn.com/gtetvomkbg.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtabhxogth.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tianlin.xyz/gtodauyymm.html


<!-- 参考信息 -->