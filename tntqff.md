代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258888.top/gtiicegolx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinghuilouyu.cn/gtoxtcgnsm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gtmkyluxyb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtyhrrljxu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtiltvtkaa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangtech.top/gtssjewudh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigfzy.top/gtbbwdejob.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuxming.cn/gtmkmfjgpx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gaohongyu789.top/gtqtidhuii.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigufen.top/gtnqbmalcg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtjfhpswir.html

JS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtzzqyzuoh.html

TS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtmyyatmit.html

Java: String.format("%03d", 7)
来源：http://hz.cdnleiting.top/gtokzvldtd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuxming.cn/gtmgaepstj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtohwdisew.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.vqdsnc.cn/gtquspcfvh.html

[E11] 反转字符串
来源：http://hz.tanke756.top/gtwcqjrsel.html

Py:   s[::-1]
来源：http://hz.yueranfly.top/gtshfrpdef.html

PHP:  strrev($s);
来源：http://hz.hammf.cn/gtmufteddh.html

JS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtgdkmafcn.html

TS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtxqmqvqkx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtqhwbphsc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tanke756.top/gtxdgydhmh.html

Ruby: s.reverse
来源：http://hz.pengpengdd.cyou/gtvicwqanv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtnjdbqlek.html

[E12] 统计某字符出现次数
来源：http://hz.dianchejie.cn/gtiaqvswsk.html

Py:   s.count("a")
来源：http://hz.guannengcc.top/gtyeucjdvz.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtlfdocvqp.html

JS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gttltjecct.html

TS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtgdsylvar.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zycfv.cn/gtldpofndd.html

Go:   strings.Count(s, "a")
来源：http://hz.hysaishi.cn/gtmglimdqe.html

Ruby: s.count("a")
来源：http://hz.yueranfly.top/gtloifysgp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gtjwbepyfz.html

[E13] 逐字符遍历
来源：http://hz.hywenlv.cn/gtoaicblpp.html

Py:   for ch in s: print(ch)
来源：http://hz.fzhhl.top/gtkvllnlfn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtfhrrvwez.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtxpeblqxp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtgwgewqpp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtfkhbwobd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.0kj1m.cn/gtijfcqslm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gtxzuolvcx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.52xcode.cn/gtxfmmssfj.html

[E14] URL 编码与 Base64
来源：http://hz.gotoacloud.top/gtfvplsdoi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.vqdsnc.cn/gtpclaiuxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.0kj1m.cn/gtbwwnnzrt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtqhojlvib.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gthlnizhlg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aizwys.cn/gthlwgkftv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dianchejie.cn/gtieyrpmkg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pengpengdd.cyou/gtdlimfadb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aibaodan.cn/gtdekrwqrd.html

[E15] HTML 转义 / 反转义
来源：http://hz.gotoacloud.top/gtpjqbxdms.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangkeji.top/gtbomehcuz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.quarkkingdee.top/gtmltdonvw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xylfe.cn/gtamegmzop.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtpmmovnkc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guannengcc.top/gtmgelewiq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtoasncuta.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtmhrellpk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cashguo.top/gtpqflzqyy.html

[E16] 数字千分位
来源：http://hz.meibo888.top/gtaeufpxit.html

Py:   f"{1234567:,}"
来源：http://hz.ppjwa.cn/gtrffvvqxd.html

PHP:  number_format(1234567);
来源：http://hz.hongshengwenyu.top/gtigrndtxe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtavwihfip.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtkjhepwll.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgfzy.top/gtuaweucun.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guowangkeji.top/gtvexbwkba.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jlsjyb.cn/gtufmeqplb.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtgxycvksg.html

[E17] 首字母大写
来源：http://hz.shzxlz.cn/gtmatmnjuw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.52xcode.cn/gtmtrrxzpd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtbefdvsnb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtytjxadde.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtiihwckzi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangtech.top/gtbecdrnmj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gtehrxborw.html

Ruby: s.capitalize
来源：http://hz.zhiwuduotai.top/gtagnejfep.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yonumen.top/gtrxlgxcqp.html

[E18] 模板占位符替换
来源：http://hz.shzxlz.cn/gtjbyifajy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuanzx.com/gtitddjzqg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.havefunace.top/gtiypvdogn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtrbjfjcbg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtdzwmxzbl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuanzx.com/gtziubdmpo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cucudq.cn/gtlusnuadb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtlmdywhpw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangdashe.top/gtotnlkcnk.html

[E19] 多行文本按行拆分
来源：http://hz.jqgfzy.top/gtecaidwli.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtkyarplwl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtbxnscosn.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtdyxrwzif.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtkibzgvyv.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtfjofsgck.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtlvdtjbdo.html

Ruby: s.lines
来源：http://hz.meibo888.top/gtndsxocfo.html

C#:   s.Split('\n')
来源：http://hz.fzhhl.top/gtbtyutpmx.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258888.top/gtytojakeg.html

Py:   if not s:
来源：http://hz.quarkkingdee.top/gtjidazrev.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtqmvpqtan.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuxming.cn/gtptotrxdg.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gthvkmzoeu.html

Java: if (s.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtyjoswdya.html

Go:   if s == "" {}
来源：http://hz.gotoacloud.top/gtbqrkukcr.html

Ruby: if s.empty?
来源：http://hz.jinyuanbaomall.cn/gtoqxetwie.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yvedp.cn/gtgdkzkrpb.html

[E21] 超长截断加省略号
来源：http://hz.nanxinkj.top/gtagytomgd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cucudq.cn/gtntqgvely.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtkvjppacl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtktrvegco.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gttbsssiif.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtcvtzkclq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigufen.top/gtobenjbal.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yongpay.top/gtxbddoihv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtqhvezsjj.html

[E22] 字节长度与字符长度
来源：http://hz.zhongyouzk.top/gtsysovclw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ehwqpu.com/gtbjcdggvz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtklntiucp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtciunnzzy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtbflexexo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangdashe.top/gtymwconyy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gogol.net.cn/gtptutfmza.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258888.top/gtuguktqqb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhongyouzk.top/gtytcogbiv.html

================================================================================
来源：http://hz.sweek.top/gtkustfrrm.html

F. 文件与目录
来源：http://hz.ybcxt.top/gthwxzaian.html

================================================================================
来源：http://hz.cheryme.top/gttzuagjrm.html

[F01] 读取整个文件
来源：http://hz.zycfv.cn/gtmoebwpmv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gthosageic.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cdnleiting.top/gtqwlmtrhq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtfgjlaglp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hammf.cn/gtkrrhkfan.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtkchxwixp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yvedp.cn/gteeymccor.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gttefwngsn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtwqgrdbtk.html

[F02] 逐行读取文件
来源：http://hz.yj20258888.top/gtqbbqtorq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtyuswbxqy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtunvpfskx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.mhx1999.top/gtgikmdiea.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtajzugkba.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtobvwlyhd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zdqjudy.top/gtwpzafulp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cucudq.cn/gtykyavize.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtcdmiamgv.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtvbetncgk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangshuangyany.cn/gtfinskhwt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.andypj.xyz/gttapgocmb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtzococxgl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtxoytxlwk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtvibjvtlz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aizwys.cn/gtmooquclk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jianghu66.top/gtiphuqqaj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtjycnvdzm.html

[F04] 追加写入文件
来源：http://hz.snrcjt.cn/gtzgtdpxke.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtkibecrrh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yueranfly.top/gtnvtpsurt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtpfwfbsgq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtxffwfiit.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jiagoushi.top/gttehtocbo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtuwpbfkdn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gteajzwivc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtcekanxiu.html

[F05] 判断文件或目录是否存在
来源：http://hz.feifeiyinyue.top/gtggbynpcr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigfzy.top/gtxsdoxnko.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gthqwussdd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtlbwuvtkf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtzvbghftm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtucgodzbp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sufxvd.cn/gtwfgnqrpb.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgufenzy.top/gtcdufvbmp.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtkxvxjegi.html

[F06] 删除文件
来源：http://hz.cqqwz.cn/gtkkamgfko.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtcnegjand.html

PHP:  unlink("a.txt");
来源：http://hz.cdnleiting.top/gtdxgsrqui.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtrwvvjrtp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtbmthlvlf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtnboqtfxn.html

Go:   os.Remove("a.txt")
来源：http://hz.yj202588.top/gtcjvrybvf.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtsxgewkbj.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtpbdowgsc.html

[F07] 创建目录（含多级）
来源：http://hz.yueranfly.top/gtlzdyowxo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gtynfpyfmu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fzhhl.top/gtdxqptqma.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtfxknlxob.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtaoxtgdcg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.mhx1999.top/gtvsrknshi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guannengcc.top/gtpdzzeoxf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.meibo888.top/gtvflcpdhd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hfpthk.cn/gtljeseurx.html

[F08] 遍历目录
来源：http://hz.316326.xyz/gtdabnucxo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gteqtozhaf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtsyqrwxoe.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtpguxybmp.html

TS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtsmgebjng.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtsowzqreu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gtnzavgvwl.html

Ruby: Dir.children("dir")
来源：http://hz.sxryk.cn/gtijiwzhpz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgufenzy.top/gttdhccdib.html

[F09] 获取文件大小
来源：http://hz.zhiwuduotai.top/gtvbdexgiz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgufenzy.top/gtgfuxmgos.html

PHP:  filesize("a.txt");
来源：http://hz.hysaishi.cn/gtjcjevarl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtpldwqvnb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtpplehkcb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gthybausyz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhaomingkeji.xyz/gtrjgjzgeg.html

Ruby: File.size("a.txt")
来源：http://hz.sweek.top/gteugblwdt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sysykeji.top/gtirgbkarz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtwxwevpsn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtjkkyetsc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gthnzbhrxe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtncpjlfti.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtdhmmsbbz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtpqmtuwgs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtjrkbgcwr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sweek.top/gtnarvlhco.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tian-w.cn/gtmofhbhmq.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gtuacncjrx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtfaqhlwbk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtjdvrvwoh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtsicjakke.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtwcmweoiu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gttdtocuhc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtdcupidja.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtpcvmdyhe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtbzletchf.html

[F12] CSV 读写
来源：http://hz.shanyushiyangtech.top/gtdlulbbgx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtthuwtayd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtzxogghii.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtlfortpew.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtptztflxx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgufenzy.top/gtxsenehzd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtgaunkwvh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gtecuxcnww.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtuhsijlgi.html

================================================================================
来源：http://hz.sweek.top/gtvnfsibtl.html

G. 面向对象
来源：http://hz.fengsongda.top/gtjexsubhc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtscvcgjkl.html

[G01] 定义类
来源：http://hz.yuxming.cn/gtogwpkgza.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtmghghtkc.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtxukiupmz.html

JS:   class User {}
来源：http://hz.havefunace.top/gtiemrdkvz.html

TS:   class User { name: string = ""; }
来源：http://hz.hfpthk.cn/gtwfbnllcj.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtxqactyen.html

Go:   type User struct { Name string }
来源：http://hz.tianlin.xyz/gthunqoiyo.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gtgizwshga.html

C#:   class User {}
来源：http://hz.nanxinkj.top/gtokhoxhft.html

[G02] 构造函数
来源：http://hz.hnxiangtu.top/gtnbtgaxqy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtwcxghmca.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cashguo.top/gtzvrvhaxa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtoxxjpamh.html

TS:   constructor(public name: string) {}
来源：http://hz.hnxiangtu.top/gtledsjyns.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtyvaeqmcf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.smart0.xyz/gtjrxaodiz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtdyztqaok.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtgddsdwse.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gtgwjosigl.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtfxernpjk.html

PHP:  public string $name = "x";
来源：http://hz.hongshengwenyu.top/gtbqkipudx.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtdrablnba.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtqnbfunqq.html

Java: private String name;
来源：http://hz.yj20258888.top/gtbvaenqlx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtedycwwdq.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtvkvgglgp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zycfv.cn/gtgoxyxyzt.html

[G04] 定义方法
来源：http://hz.zhongyouzk.top/gtfgblwypj.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtnttlwtac.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtxkeuulrv.html

JS:   greet() { return this.name; }
来源：http://hz.yvedp.cn/gtjprbknmt.html

TS:   greet(): string { return this.name; }
来源：http://hz.fengsongda.top/gtwduxkjdk.html

Java: String greet() { return name; }
来源：http://hz.chenjidiqi.icu/gtivmlxsbh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pycfn.com/gtjuphqipj.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtzbzmfajj.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtlrxobysc.html

[G05] 继承
来源：http://hz.ydjk.org.cn/gtcozcywfd.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtxnvyiaak.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtijszzilm.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtlsssjupo.html

TS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtpencsoov.html

Java: class Admin extends User {}
来源：http://hz.mhx1999.top/gtgcfomojj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gtqczfdulk.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtrwdtukhi.html

C#:   class Admin : User {}
来源：http://hz.jianghu66.top/gtdthhnnwd.html

[G06] 重写方法
来源：http://hz.snrcjt.cn/gtazajxgww.html

Py:   def greet(self): return "admin"
来源：http://hz.snrcjt.cn/gtjwjqjyky.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtrenjovxi.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtsuiwmcby.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtcjigndgy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtamimxits.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtthlghmyv.html

Ruby: def greet; "admin"; end
来源：http://hz.xziqi.cn/gtzfsjgjgw.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtvcnneude.html

[G07] 调用父类方法
来源：http://hz.cheryme.top/gtexmtrlel.html

Py:   super().greet()
来源：http://hz.zhengqikj.top/gtwquphylc.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtkjqivikh.html

JS:   super.greet();
来源：http://hz.gotoacloud.top/gtshhxckjc.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtckvjyjva.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gtojeraxiv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zycfv.cn/gttwwvsypf.html


<!-- 参考信息 -->