代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.ydzc1.top/gtsfleagvq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.redwolf501.top/gtfgpoqras.html

[E08] 数组按分隔符合并
来源：http://hz.hysaishi.cn/gtidvqkogm.html

Py:   ",".join(items)
来源：http://hz.0kj1m.cn/gtrbxpbqfg.html

PHP:  implode(",", $items);
来源：http://hz.zhaomingkeji.xyz/gthhfjspet.html

JS:   items.join(",")
来源：http://hz.zhixingplan.top/gthtlvnsiu.html

TS:   items.join(",")
来源：http://hz.tanke756.top/gtebqlhdel.html

Java: String.join(",", items)
来源：http://hz.gaohongyu789.top/gtjipfwmkj.html

Go:   strings.Join(items, ",")
来源：http://hz.guowangkeji.top/gtpizmkype.html

Ruby: items.join(",")
来源：http://hz.cqqwz.cn/gtxqkluibq.html

C#:   string.Join(",", items)
来源：http://hz.gaohongyu789.top/gtebeveddb.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtyvdyqzce.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gtdrrfkdem.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtrmdlpvxz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtnrbzcvtj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtfxyldese.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.havefunace.top/gtovhticnw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtkhtclwzg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtdhbjbhvu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.svipenyu.cn/gtnixgsnso.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hammf.cn/gtxmcvsrtp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnqzz.top/gtmzbzxafc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtozzagstz.html

JS:   "7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtzebbbshg.html

TS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtfnbjziob.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtvkqnflrx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtpniqlhdj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtmjuoaspz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhongyouzk.top/gthuvdubls.html

[E11] 反转字符串
来源：http://hz.52xcode.cn/gtqxmposiq.html

Py:   s[::-1]
来源：http://hz.iojbl.cn/gtsqylflmd.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtkuzvcadn.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtpjrwaeui.html

TS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtsgahiqnx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtvwoqdhcb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj202588.top/gtkjqfrvhg.html

Ruby: s.reverse
来源：http://hz.yuxming.cn/gtyuahdkmq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtzngvixxh.html

[E12] 统计某字符出现次数
来源：http://hz.guannengcc.top/gttopufahj.html

Py:   s.count("a")
来源：http://hz.zhaomingkeji.xyz/gtkohpkxbm.html

PHP:  substr_count($s, "a");
来源：http://hz.guowangkeji.top/gtseawoqex.html

JS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtnkckujjq.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtalbnpxxs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtpphixmlk.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtwwmfwind.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtyhnjyrjg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtfcvfmwha.html

[E13] 逐字符遍历
来源：http://hz.yuxming.cn/gtpgtixstm.html

Py:   for ch in s: print(ch)
来源：http://hz.dianchejie.cn/gtdzywjpwe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sxryk.cn/gtarwukxhs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtylswtluw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtcozheuku.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.dashuyun.cn/gtfsaekncv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gthdesnspm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xingfuxueyuan.xyz/gtftkiyrll.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gtnjvbgdlz.html

[E14] URL 编码与 Base64
来源：http://hz.shzxlz.cn/gtdgjiibrt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.9152youxi.cn/gtjvywiqxt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtrximizko.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangtech.top/gtovhwdcpo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sysykeji.top/gtjucvhanw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtxeyhpgts.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ybcxt.top/gtvkccciyh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daxiang520.top/gtbxqsftge.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.andypj.xyz/gtzgymgpam.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gthyxiilqv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgufenzy.top/gtvdmniyoq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xingfuxueyuan.xyz/gtoeinyklq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hammf.cn/gtlwegtjsl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jlsjyb.cn/gtohaidsyt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shangyingyoupin.top/gtugtefnar.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhongyouzk.top/gthfmxnuep.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtjkewokjp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pengpengdd.cyou/gtznuefrbt.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtopogpvnh.html

Py:   f"{1234567:,}"
来源：http://hz.jinyuanbaomall.cn/gtsgnwieyb.html

PHP:  number_format(1234567);
来源：http://hz.cdnleiting.top/gtaqscpkpz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtoyweykku.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtcenddsig.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nwbrower.top/gtzzovtndd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtlxcinukg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhoulong.xyz/gtewljiizv.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgfzy.top/gtzlczqvuv.html

[E17] 首字母大写
来源：http://hz.havefunace.top/gtmkfgkdml.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gzhubu.top/gtdsxhxnxl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtpryndlfr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtlykrdtyh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtgsqgrjts.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gtyzzmqnyp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gthpsvylix.html

Ruby: s.capitalize
来源：http://hz.xinyue.icu/gtathonqjy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.meibo888.top/gtydobdaan.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtbdwtyfuc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.feifeiyinyue.top/gtmckzqrtc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fengsongda.top/gtumzkpvrl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtzpbddsxd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtewdadlze.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ybcxt.top/gtpqgjidbo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cucudq.cn/gtvvnksozo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aibaodan.cn/gtrhhoujib.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtyagbczqx.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtiylhftyl.html

Py:   s.splitlines()
来源：http://hz.gaohongyu789.top/gtndpnxjkp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258.top/gtzspnmgnq.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gthuvvkzjh.html

TS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtgqbougmv.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gttcnvvfte.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gthppqlwem.html

Ruby: s.lines
来源：http://hz.ydzc1.top/gtlrvijqrv.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtxfnzrzrn.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangtech.top/gtnoiyshno.html

Py:   if not s:
来源：http://hz.cashguo.top/gtzkuljwkd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hammf.cn/gtpuoofdnt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtqlzwzsfl.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtssniioab.html

Java: if (s.isEmpty()) {}
来源：http://hz.redwolf501.top/gtvcwcsgmr.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gtiydphwzh.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gteeisslbh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtjmkwhnvs.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gtecnxbdcu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jlsjyb.cn/gtbiohwcsu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hongshengwenyu.top/gtardtxtbd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtmrlljkvr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtktmswnvk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtgkauxdgf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guannengcc.top/gtakihrufb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gotoacloud.top/gtjcoycwni.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.andypj.xyz/gtouyfyoas.html

[E22] 字节长度与字符长度
来源：http://hz.xuanzx.com/gtwwrtkgfd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.vqdsnc.cn/gtytjxheca.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtqnmwgdzd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtckftqnkh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtfudkirjx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jlsjyb.cn/gtamsjezcb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtdhqsoaio.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtogzfazou.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shuidangran.top/gtyxutdnny.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtynpwckjh.html

F. 文件与目录
来源：http://hz.andypj.xyz/gtlygydbng.html

================================================================================
来源：http://hz.jlsjyb.cn/gtfssqjsvt.html

[F01] 读取整个文件
来源：http://hz.ydjk.org.cn/gtwhfxzlpg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtotigxvhc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jlsjyb.cn/gtllxqfqpx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gticdwiphm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuanzx.com/gtwyqohwta.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtiefcxdqk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtwartmafq.html

Ruby: File.read("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtsixxtrhe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtcdhzygfy.html

[F02] 逐行读取文件
来源：http://hz.redwolf501.top/gtylvkmeyn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhiwuduotai.top/gtjjxtyjkh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtktpjqroq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtfbhcwwkn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtzxqcidmh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtrwcywkro.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.0kj1m.cn/gtkqdokyeh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.redwolf501.top/gtuznatmuh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtpzvyucvr.html

[F03] 写入文件（覆盖）
来源：http://hz.sufxvd.cn/gtbvfiehwc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gtmivfvuhp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtbgklrkfl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gthnejxmwi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtzlfnnhyf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cqqwz.cn/gtmyhsksol.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtgemwjanj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtdazbdhzr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zdqjudy.top/gtjryinopl.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangtech.top/gthiwbihsb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gtpswninjb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xziqi.cn/gtcizxnyuy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtibwwqahx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cucudq.cn/gtamkswmbd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhixingplan.top/gttfajfyxo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj202588.top/gtdboqciab.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gogol.net.cn/gtzxoulipa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinyuanbaomall.cn/gtxnoacttt.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtgazjmrfn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cheryme.top/gtvxdncfvp.html

PHP:  file_exists("a.txt");
来源：http://hz.snrcjt.cn/gtjwcwhcbn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtybbglnde.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtivvnanbz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtwrkxwtls.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yangfankeji.com/gtouqaedct.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangdashe.top/gtkvgvvush.html

C#:   File.Exists("a.txt")
来源：http://hz.daxiang520.top/gtfmmtumef.html

[F06] 删除文件
来源：http://hz.c1oappe.top/gtdbjmuedy.html

Py:   os.remove("a.txt")
来源：http://hz.tianlin.xyz/gtemyfbcrn.html

PHP:  unlink("a.txt");
来源：http://hz.zycfv.cn/gtdavhrqmt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtswjyllvd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gttbaqtulj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gthrprskwc.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtogthyzhf.html

Ruby: File.delete("a.txt")
来源：http://hz.wangdashe.top/gtxywejatr.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtxtvtbehb.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gtousvuyjn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydzc1.top/gtmliuhoia.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.kuanghao11.cn/gttuuknfrj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gttkatwkuq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtwbgminkz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yonumen.top/gtxwixbgmv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.quarkkingdee.top/gtfvqepxge.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtovntccny.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sweek.top/gtfpglzngx.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtbswcasju.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtrsglkjpz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtxwhrwetn.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gttplicpba.html

TS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtivrewbdi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtfuowjbqd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.havefunace.top/gthdylaoyu.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gtyjlkwlxo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenjidiqi.icu/gtesnftpls.html

[F09] 获取文件大小
来源：http://hz.nwbrower.top/gtperrwcez.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtqmjsvgix.html

PHP:  filesize("a.txt");
来源：http://hz.ydjk.org.cn/gtrxkhdsru.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtzadjbidt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtnvakpbaw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtagyryprt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cdnleiting.top/gtjbwtfemx.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gtdtcwrtoo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cucudq.cn/gttbypubqz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cqqwz.cn/gteylfswzw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtghvdapat.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtjlghbcyv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtrmwqrpyy.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gtkkbkycgf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cucudq.cn/gtwzdmplwm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dianchejie.cn/gtrtigesxm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtwuwrrces.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtuvxqyrug.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtlenenqhd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtnhnvmgzv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhijiandao.cn/gtarwgdzbc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtoqdurcvn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtuapojkix.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhixingplan.top/gtbchxkklw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtjqjaqeew.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtbpoqqxhc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangkeji.top/gthaaizlhx.html

[F12] CSV 读写
来源：http://hz.0kj1m.cn/gtbbzfjigy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gttsjcjhso.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtipmdutqq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.c1oappe.top/gtugdlhbob.html

TS:   // 同上
来源：http://hz.birdmap.top/gtlkbjbqgx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtnfxdmjrm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangdashe.top/gtbksmaqxb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yongpay.top/gtymktjovi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtjjsnxtqv.html

================================================================================
来源：http://hz.52xcode.cn/gtmkvanjas.html

G. 面向对象
来源：http://hz.ivvv.top/gtdgdkwgwe.html

================================================================================
来源：http://hz.daxiang520.top/gtdvqxmplj.html

[G01] 定义类
来源：http://hz.yanxiufei.cn/gtgjaelmee.html

Py:   class User: pass
来源：http://hz.yuxming.cn/gtjczbuwvw.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtyjkqyvmy.html

JS:   class User {}
来源：http://hz.shuidangran.top/gtklktwufo.html

TS:   class User { name: string = ""; }
来源：http://hz.gotoacloud.top/gtrervehqy.html

Java: class User {}
来源：http://hz.gogol.net.cn/gtewnuhect.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtndwvnfig.html

Ruby: class User; end
来源：http://hz.iojbl.cn/gtsdkxmzvt.html

C#:   class User {}
来源：http://hz.pengpengdd.cyou/gtzjcscfkd.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtfaqofsvr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.meibo888.top/gtownyejby.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pengpengdd.cyou/gtumepgxph.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtuynvkmny.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtehfctytu.html

Java: User(String name) { this.name = name; }
来源：http://hz.smart0.xyz/gtolmntnyy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hongshengwenyu.top/gtirkbeudm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtkexrxeoa.html

C#:   public User(string name) { Name = name; }
来源：http://hz.smart0.xyz/gtjjohbysj.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtqdfjbkuv.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtmhifmgrt.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtvebnxtvq.html

JS:   this.name = "x";
来源：http://hz.havefunace.top/gtgxzgjdlb.html

TS:   name: string = "x";
来源：http://hz.hammf.cn/gtdyhlcsmp.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtzkysbeen.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtlxyewozh.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtwybziohr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtzkbbwnbi.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtjvpfkthu.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gteupkncog.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtczgasrgp.html

JS:   greet() { return this.name; }
来源：http://hz.zhoulong.xyz/gtommmmpoe.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtrejjyfli.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtggimfogn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtmdgerbkv.html

Ruby: def greet; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtdqqcnbep.html

C#:   public string Greet() => Name;
来源：http://hz.ybcxt.top/gtatqulfbo.html

[G05] 继承
来源：http://hz.mhx1999.top/gtrijminiz.html

Py:   class Admin(User): pass
来源：http://hz.iojbl.cn/gtizkglvzo.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtarpnxhyb.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtnxuuqfah.html

TS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtkkjyhjhh.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtfpdzjhoi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtgsmfakmg.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gtuwjfoazr.html

C#:   class Admin : User {}
来源：http://hz.vqdsnc.cn/gtxxlutper.html

[G06] 重写方法
来源：http://hz.cashguo.top/gtmcgzxhsw.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtilejgfdk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtvvrbcbhp.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gttwsrcpyp.html


<!-- 参考信息 -->