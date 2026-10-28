代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gtniizhelo.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtfkmzenqr.html

TS:   items.join(",")
来源：http://hz.smart0.xyz/gttatmcbbw.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtlygvvrdm.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtrqnimobu.html

Ruby: items.join(",")
来源：http://hz.tianlin.xyz/gtvemkjecd.html

C#:   string.Join(",", items)
来源：http://hz.jinqigfzy.top/gtpixdnqhx.html

[E09] 去除所有空白字符
来源：http://hz.shzxlz.cn/gtbvuancjd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hfpthk.cn/gtqqbxbuij.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shzxlz.cn/gtedmeozoj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtzqwxzccj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gtxnsciijd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtqlgqpbmi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtwbuvzncy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangdashe.top/gtlnezzvpe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnqzz.top/gtstqpqyaa.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sysykeji.top/gtrktvwvdk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtmnmpnogi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.andypj.xyz/gtoxgkpspy.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtclklrnzj.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtkuocisgz.html

Java: String.format("%03d", 7)
来源：http://hz.yuxming.cn/gtcgqadxzv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtyajuxqwq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258.top/gtumtlldhj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shuidangran.top/gtyiaqgusp.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtfuhdyjdw.html

Py:   s[::-1]
来源：http://hz.zhiwuduotai.top/gtiowzsabz.html

PHP:  strrev($s);
来源：http://hz.chenzaomai.com/gtszseishy.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gttuuhtxlm.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtbizenvnk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtpczqmdfc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xinyue.icu/gtvfgnaukr.html

Ruby: s.reverse
来源：http://hz.shangyingyoupin.top/gtcjsjcdxa.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtjdgrygjz.html

[E12] 统计某字符出现次数
来源：http://hz.jinqigufen.top/gttlcqnioo.html

Py:   s.count("a")
来源：http://hz.meibo888.top/gtxmmsywfs.html

PHP:  substr_count($s, "a");
来源：http://hz.daria6918.cn/gtsirjpswt.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtopamubju.html

TS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gttvjuzktk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtsuckowcf.html

Go:   strings.Count(s, "a")
来源：http://hz.tian-w.cn/gtwvaukrib.html

Ruby: s.count("a")
来源：http://hz.yuanzhike.top/gtmhgdbyye.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gtfagunkjz.html

[E13] 逐字符遍历
来源：http://hz.svipenyu.cn/gttjhvgaka.html

Py:   for ch in s: print(ch)
来源：http://hz.bjfxy.top/gtokclrjbi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yangfankeji.com/gtgzcqomjo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenlongwang.top/gtquwoiisk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtzbrzxqri.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sxryk.cn/gtivojygfi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.iojbl.cn/gtchiobnxc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ehwqpu.com/gtfwhfdzmv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigfzy.top/gtahbfxexw.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtfnyvmjmm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtuuwfwbzt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtcenlpylf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yvedp.cn/gtbkmlfvbh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pycfn.com/gthukraktk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daria6918.cn/gtsfviioje.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yonumen.top/gtjqspsmay.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cashguo.top/gtkvyctthl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtucjmomwb.html

[E15] HTML 转义 / 反转义
来源：http://hz.yongpay.top/gtgefdqdor.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnxiangtu.top/gtdabniphw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtikhdwysz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aibaodan.cn/gtfuoibssw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ywan-chungtsiang.top/gtxiedzljw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jiagoushi.top/gtveudxkfn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtnxqiwiuk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aibaodan.cn/gtgirvbewk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhoulong.xyz/gtrpltzzrc.html

[E16] 数字千分位
来源：http://hz.tanke756.top/gtfrgafntu.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtgcvolxwz.html

PHP:  number_format(1234567);
来源：http://hz.daria6918.cn/gtocvmhkof.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yueranfly.top/gtpowgxblw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtyxngzvwf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gaohongyu789.top/gtezqwgyns.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gtjznecftj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.feifeiyinyue.top/gtdkpfwvhr.html

C#:   1234567.ToString("N0")
来源：http://hz.xingfuxueyuan.xyz/gtgpnzjmkj.html

[E17] 首字母大写
来源：http://hz.cucudq.cn/gtksftjggp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuanzhike.top/gtjduodazt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sweek.top/gtrwaxtocf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ybcxt.top/gtbbtsrhzh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtqhilhoro.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangdashe.top/gtgxptwhog.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aizwys.cn/gtjrrgwzmz.html

Ruby: s.capitalize
来源：http://hz.shanyushiyangkeji.top/gtmbpnrhdd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nwbrower.top/gtugpakqat.html

[E18] 模板占位符替换
来源：http://hz.pycfn.com/gtsdcdncnz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gtxggicrsf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenzaomai.com/gtlkkapzxu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtrkmgvcqa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtkxswtqng.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhijiandao.cn/gtfcbijiie.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fzhhl.top/gtzomftzir.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gtibselrmi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gthxtodjbm.html

[E19] 多行文本按行拆分
来源：http://hz.tianlin.xyz/gtrbpscbok.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gtskfrdgtj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangshuangyany.cn/gtbwjsipvv.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhaomingkeji.xyz/gtzeqpwila.html

TS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtebbyfdhx.html

Java: s.lines().toList()
来源：http://hz.jinqigufen.top/gtvvgoqplw.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtsebzlrlp.html

Ruby: s.lines
来源：http://hz.quarkkingdee.top/gtssdvznsb.html

C#:   s.Split('\n')
来源：http://hz.zhengqikj.top/gteyahfngc.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtkqppswea.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtoichasjn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhongyouzk.top/gtjzbyxbvg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtbkhcoshy.html

TS:   if (s === "") {}
来源：http://hz.gaohongyu789.top/gtjdntpsly.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gtqfolvcyv.html

Go:   if s == "" {}
来源：http://hz.zhixingplan.top/gtobtghpjs.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtlrkdfuka.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yueranfly.top/gtsbhcydjr.html

[E21] 超长截断加省略号
来源：http://hz.wangdashe.top/gtrwsyhzht.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zycfv.cn/gtpsahsrev.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuanzhike.top/gtuejayepc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtrhmckuxd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtzbecgnpb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtbzjlzfjr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.feifeiyinyue.top/gtvpwubzxy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.havefunace.top/gtqnrjjuuz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gtkarysljf.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gtpxksskvf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guannengcc.top/gtyqoeszpd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtuqkesrzm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gtnzjvbxux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtspliijlg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hongshengwenyu.top/gtkdtdtjsl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ehwqpu.com/gtxfzekcuo.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnqzz.top/gtagxvpssd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinghuilouyu.cn/gtysgugepj.html

================================================================================
来源：http://hz.zdqjudy.top/gtxrahpuky.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gtueticdub.html

================================================================================
来源：http://hz.xuanzx.com/gtboashtho.html

[F01] 读取整个文件
来源：http://hz.xziqi.cn/gtzofyicth.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtankvdogk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gtjqdofkqg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hysaishi.cn/gtmymztmco.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtucloecgl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtdyxaaeln.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jlsjyb.cn/gtxqmpbufo.html

Ruby: File.read("a.txt")
来源：http://hz.xuetiantiany.cn/gtagrarmee.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtppjpvwnk.html

[F02] 逐行读取文件
来源：http://hz.xingfuxueyuan.xyz/gtwzplauzw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xziqi.cn/gtmxrmphzh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.mhx1999.top/gthyiebzqx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtgelqwkxn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtwxrqqmls.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shangyingyoupin.top/gthndgjncc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dianchejie.cn/gtxajbmtgf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dashuyun.cn/gtubbulkdm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pycfn.com/gthdorlmto.html

[F03] 写入文件（覆盖）
来源：http://hz.yj202588.top/gtfasmqvev.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gtktxcqpwu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtzsueynds.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtzrchqhos.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtgntdtzno.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigfzy.top/gtrqtgjdkf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gtthzxrbii.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtwbjzhbfd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtqwqknabs.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtshwmlgxd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gthzitfkqn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtkgeypkdq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtakljokvm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtlzptmivs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtcozwizwx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.bjfxy.top/gtqlhljjux.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shuidangran.top/gtjslclipm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aizwys.cn/gtouaatluu.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gtfrgejnaq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gtbgoejamv.html

PHP:  file_exists("a.txt");
来源：http://hz.cashguo.top/gtsuogjriq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtsopjjgbu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtwucuxjdo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtiaknwnie.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtqhwbcwqn.html

Ruby: File.exist?("a.txt")
来源：http://hz.shangyingyoupin.top/gtlihdatuq.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtwuhgfcuh.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtmthlwvid.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtalhwwpko.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtnaaiaryx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtptbjqueb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtviofybms.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtcwwibtwo.html

Go:   os.Remove("a.txt")
来源：http://hz.ybcxt.top/gtcynjdmhv.html

Ruby: File.delete("a.txt")
来源：http://hz.hfpthk.cn/gtzqznnffs.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtfdrwoqfr.html

[F07] 创建目录（含多级）
来源：http://hz.hywenlv.cn/gtgokxplrq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.iojbl.cn/gtdwklkwgs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daria6918.cn/gtuwnagehj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gthuahrlxm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtibcjxroo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shuidangran.top/gtvkxigowi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xingfuxueyuan.xyz/gtxheyooqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gtqvtlrtmt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtnzthixuj.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gtadogpthx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.mhx1999.top/gtnkjjmtiw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtviasdfse.html

JS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtgkmonnnf.html

TS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gtmdomajrl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gthzepkhkp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxinkj.top/gttogsvqyk.html

Ruby: Dir.children("dir")
来源：http://hz.jianghu66.top/gtnwqjbagc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtqwjqobeo.html

[F09] 获取文件大小
来源：http://hz.zhongyouzk.top/gtwbxeuecf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fengsongda.top/gtxlnakafg.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtgojmzcpx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xylfe.cn/gtlvolmvmf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtzgueicnz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtzbodtulf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.vqdsnc.cn/gtslykrzcn.html

Ruby: File.size("a.txt")
来源：http://hz.ehwqpu.com/gtzmelonde.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258888.top/gtdzzsxlgv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daxiang520.top/gticpmovpf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtjjyaidyz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangtech.top/gtcueroyrm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtjkdrzomz.html

TS:   path.extname("a.txt")
来源：http://hz.guannengcc.top/gtwweouglr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtttxihszd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shuidangran.top/gttiwjgbnm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtkvfcwzwb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hywenlv.cn/gtlkzcicjg.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtnezqqncy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtcuewzsoa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtakcrmbxd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtvscruqgk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtxvubqgtz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shuidangran.top/gtkwcyekka.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtrrqhpebb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtwyozlzdj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daxiang520.top/gtsrnpojjl.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtnaixlakj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shangyingyoupin.top/gtpzxyfczl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gtpcymkkqu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxinkj.top/gtcbwwmfmn.html

TS:   // 同上
来源：http://hz.aibaodan.cn/gtthsaqtna.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnxiangtu.top/gtamfsiudh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtqpdnyntd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nwbrower.top/gtuptcnkdy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gttdozirfx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtowhmbkko.html

G. 面向对象
来源：http://hz.yonumen.top/gtezpsvzlz.html

================================================================================
来源：http://hz.tanke756.top/gtjarfeloz.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtfjgxegug.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtxnihuaek.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtupffxsmr.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtdobyctqx.html

TS:   class User { name: string = ""; }
来源：http://hz.pengpengdd.cyou/gtyqvoytfz.html

Java: class User {}
来源：http://hz.feifeiyinyue.top/gtyibxqyle.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtupwbuqvv.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtoactfrdr.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gtqfimpslg.html

[G02] 构造函数
来源：http://hz.chenjidiqi.icu/gtpitlstwo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.andypj.xyz/gtobueuryt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gaohongyu789.top/gtmpapsaoq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtmavfjphz.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtdjykypsb.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtvsivkvbw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xziqi.cn/gtgpfqcmad.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnqzz.top/gtwflincyh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fengsongda.top/gtdejfrgtt.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gtlxzhpxrc.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtorfovzeq.html

PHP:  public string $name = "x";
来源：http://hz.ehwqpu.com/gtiisammwz.html

JS:   this.name = "x";
来源：http://hz.chenjidiqi.icu/gtioyzverh.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtayosphnx.html

Java: private String name;
来源：http://hz.gzhubu.top/gtznxglqvr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gtncecjbyf.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtbzxzbhca.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtfsmnqzxd.html

[G04] 定义方法
来源：http://hz.yuanzhike.top/gtaavlzahv.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gttiwodhts.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtbkugbnla.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gteztsapew.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtkxeoocbg.html

Java: String greet() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtoussudwm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtugappers.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtotscylmt.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gttgrphzgr.html

[G05] 继承
来源：http://hz.nanxinkj.top/gtkuahcrzm.html

Py:   class Admin(User): pass
来源：http://hz.ywan-chungtsiang.top/gtjrcmzffm.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gttqxvbfoe.html

JS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtjnfhvcji.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtxmcbwayp.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtsyslyldf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.316326.xyz/gtiaavdrqw.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gttrpflgmh.html

C#:   class Admin : User {}
来源：http://hz.shangyingyoupin.top/gtjhnsqxza.html

[G06] 重写方法
来源：http://hz.chenzaomai.com/gtbgyivhdg.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258.top/gtpbqfpeyg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtaqioqgsr.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gttarmagqo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtcurmurat.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtvpbqfhnf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.redwolf501.top/gtewdtgejd.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtlnjvtsgb.html


<!-- 参考信息 -->