代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hysaishi.cn/gtsazcubll.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xuanzx.com/gtgipnbfte.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtjstltrdj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtldhglnlb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtyjlcdwvd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtcafxnlon.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.birdmap.top/gtqqpihqby.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fengsongda.top/gtpdvmdxfe.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtpjytyyav.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtvhphesfz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtesuckvvf.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtytmibatw.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtzxzgwlmv.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtrcbzofmw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxuanxn.top/gtpznaktuj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gtluekncax.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gthceeemyd.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtnlvhpbwn.html

Py:   s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtudvxgpqj.html

PHP:  strrev($s);
来源：http://hz.zdqjudy.top/gtnablobdr.html

JS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtnytlvsgu.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtaxubkzvv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuanzx.com/gtxbnpcixh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtldpqfjpe.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtjqhetnlq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtkrparcsn.html

[E12] 统计某字符出现次数
来源：http://hz.bjfxy.top/gtlralfrvq.html

Py:   s.count("a")
来源：http://hz.shangyingyoupin.top/gtdffxwdzy.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtczczydaq.html

JS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtvwmplelp.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtihzwxcck.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hywenlv.cn/gtpgyjxzze.html

Go:   strings.Count(s, "a")
来源：http://hz.daria6918.cn/gtskdxeewl.html

Ruby: s.count("a")
来源：http://hz.jqgufenzy.top/gtaddeofzr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtsinxzkqj.html

[E13] 逐字符遍历
来源：http://hz.chenjidiqi.icu/gtoybemivu.html

Py:   for ch in s: print(ch)
来源：http://hz.yvedp.cn/gtqoawcjhc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gotoacloud.top/gtruvqgjzt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtunhojuug.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtzkuelfkr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj202588.top/gtyizixafp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuxming.cn/gtmiujnjco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xinyue.icu/gtwylvbazl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtzcfuticd.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gthfmnymbo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtjqvhusqz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.9152youxi.cn/gtnhznhqnb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenzaomai.com/gtmkzrqltc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgufenzy.top/gtywsxrcil.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtpenpuarv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtsnfcvxkp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jiagoushi.top/gtdwohzfsj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ppjwa.cn/gtgmwkzrbf.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtkpodrgcm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhaomingkeji.xyz/gtqqwvhvgw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jyoumei.cn/gtfxejgtma.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ivvv.top/gtmeyzbymx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhoulong.xyz/gtzvpwbjdi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxinkj.top/gtithaxdig.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jianghu66.top/gtboidthyu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zdqjudy.top/gtoklsqvab.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.vqdsnc.cn/gtshqrrclr.html

[E16] 数字千分位
来源：http://hz.nanxuanxn.top/gtkrniqqfh.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gtosznuelg.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gthyvqjgjv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gttrrjcksv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtlxbljkvz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtzqqjqtab.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtxkrevcee.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtqipuiemv.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gtbqdxdhrl.html

[E17] 首字母大写
来源：http://hz.gaohongyu789.top/gtaqksepxo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.havefunace.top/gtrxqskwcb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gttmdkxvaz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtdvgbrgtx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtyhsymbpg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtwcnsqcjt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xylfe.cn/gtjuhgdfwo.html

Ruby: s.capitalize
来源：http://hz.gogol.net.cn/gtcoaenzpw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gtjtkgwhlp.html

[E18] 模板占位符替换
来源：http://hz.jlsjyb.cn/gthkxklttb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnxiangtu.top/gttovdkssa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhongyouzk.top/gtqzpwvqgk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtjpvihdez.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtpwlatjnj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtzouewkfi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gtfrgzyfus.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.wangshuangyany.cn/gtmiixdywd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dashuyun.cn/gtuppdazxt.html

[E19] 多行文本按行拆分
来源：http://hz.iojbl.cn/gtnhntqhov.html

Py:   s.splitlines()
来源：http://hz.zycfv.cn/gtnqipnzzn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtcpbwzmpj.html

JS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtoibaegot.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtmjybuzau.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtvqszokmu.html

Go:   strings.Split(s, "\n")
来源：http://hz.nwbrower.top/gtmqqclmsu.html

Ruby: s.lines
来源：http://hz.shuidangran.top/gtgszrfnup.html

C#:   s.Split('\n')
来源：http://hz.zdqjudy.top/gtowxztuks.html

[E20] 判断字符串是否为空
来源：http://hz.ppjwa.cn/gtrhlpxikp.html

Py:   if not s:
来源：http://hz.sweek.top/gtpnsdpebr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtwfhnvzsf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.mhx1999.top/gtlrhxyosp.html

TS:   if (s === "") {}
来源：http://hz.gaohongyu789.top/gtscfrkhoh.html

Java: if (s.isEmpty()) {}
来源：http://hz.pengpengdd.cyou/gtrszrtevt.html

Go:   if s == "" {}
来源：http://hz.jinqigufen.top/gtbrljmiol.html

Ruby: if s.empty?
来源：http://hz.jinqigfzy.top/gtymosidjs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinyuanbaomall.cn/gtyfdrpcvz.html

[E21] 超长截断加省略号
来源：http://hz.daria6918.cn/gttltwbftf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtifkbltrb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtepmhhtyf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtomsgeulf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtfmwgbdlh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtovopdbdm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jiagoushi.top/gtmrwajjxb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtgpxdmhxf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtkbcfbvvt.html

[E22] 字节长度与字符长度
来源：http://hz.gogol.net.cn/gtmtghnswm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gtbasbsvje.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtvrjbfshs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.9152youxi.cn/gtuydhbaqe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtpriuykad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtcshoecta.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sweek.top/gtqyfkjihr.html

Ruby: s.bytesize;  s.length
来源：http://hz.meibo888.top/gtzkwexnjc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gtgduiuxmy.html

================================================================================
来源：http://hz.zycfv.cn/gtgvkcahep.html

F. 文件与目录
来源：http://hz.chenjidiqi.icu/gtbfjzzalu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkhqcchnw.html

[F01] 读取整个文件
来源：http://hz.tanke756.top/gthjrvthia.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gttfzobkeq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydjk.org.cn/gtnhmcyyvc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtibulickv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtdyoqssqj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtcnebnpmi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.redwolf501.top/gtrbfsfkcu.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangtech.top/gtxkueemsy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtvgnvngll.html

[F02] 逐行读取文件
来源：http://hz.hysaishi.cn/gtqeazwfkp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtoptlwxjy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtcanmswfe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtjeqecowg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangdashe.top/gtlrniamnm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gterzzalhc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tianlin.xyz/gtkcpngvjn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.havefunace.top/gtomnyccvw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhaomingkeji.xyz/gtkwwrpzgn.html

[F03] 写入文件（覆盖）
来源：http://hz.smart0.xyz/gtabjpxwfn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shangyingyoupin.top/gtaqyxgjug.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zycfv.cn/gtbiopodfw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtaxpnulmk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtlvupgpll.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xylfe.cn/gtmenrigjk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.smart0.xyz/gtiachaxml.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ywan-chungtsiang.top/gthhrnalri.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtclzrtfak.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangtech.top/gtuzshfphj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtsljlpsxq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yonumen.top/gtzfyxhgus.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtyebzsbeh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtqfdsufqr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtwnhsydjc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtxevowrfr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shuidangran.top/gtqakgiegh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtjifctezm.html

[F05] 判断文件或目录是否存在
来源：http://hz.jianghu66.top/gtjwzuovld.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtdkfvmodv.html

PHP:  file_exists("a.txt");
来源：http://hz.yueranfly.top/gtcoyfamqc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtmmuiqczn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gtlrwvsalq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtpvbsuyow.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yangfankeji.com/gtixyfvhoi.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtuniimqxh.html

C#:   File.Exists("a.txt")
来源：http://hz.andypj.xyz/gtbzcowzct.html

[F06] 删除文件
来源：http://hz.zycfv.cn/gtyrtvcrrk.html

Py:   os.remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtyocerffz.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gtxjpaodzh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gthagbbynm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtwoadeuqp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtnovfoawn.html

Go:   os.Remove("a.txt")
来源：http://hz.fengsongda.top/gtlxmpkrla.html

Ruby: File.delete("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtmvkxitzg.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtzddsutwi.html

[F07] 创建目录（含多级）
来源：http://hz.sxryk.cn/gtqmxinrum.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tanke756.top/gtdvcriqmo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtjojxwmvl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtmgtcjaoh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shzxlz.cn/gtpcekpqoj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gzhubu.top/gtxkjrwhiy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gttwxylhmt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtjnjbestr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xziqi.cn/gtxdtdlzrm.html

[F08] 遍历目录
来源：http://hz.xuetiantiany.cn/gtyeiaormj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtmleqwpqb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtjpcolvrr.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtlnffkskg.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtymofyspv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtkwhddkvy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hywenlv.cn/gtjiysyqvy.html

Ruby: Dir.children("dir")
来源：http://hz.jqgufenzy.top/gtmeqnbhfg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuanzx.com/gtfjnzjmtf.html

[F09] 获取文件大小
来源：http://hz.yuanzhike.top/gtuhclcrxo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnqzz.top/gtqktkowwz.html

PHP:  filesize("a.txt");
来源：http://hz.tianlin.xyz/gtriulrtzv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtwwnhthyl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtizvzinoh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtgbiuhzih.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gzhubu.top/gtqivvqhxi.html

Ruby: File.size("a.txt")
来源：http://hz.c1oappe.top/gtfkpeuobf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtwmoujtbe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gtnnytybxu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtnbmryjhv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gtrcqznnzi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtnahnzpcg.html

TS:   path.extname("a.txt")
来源：http://hz.cqqwz.cn/gtaratdetc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gtvpvzvndr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gthekkelam.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtyuduxmcb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtgdeupmrn.html

[F11] 复制与移动文件
来源：http://hz.jiagoushi.top/gtvytytmze.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtoxjbjakt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj202588.top/gtvszjpvep.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtjutokkrt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtovvvxppt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtpvdsqqcj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cdnleiting.top/gtsaftpvgx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtzipawixb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xylfe.cn/gtlteaanhf.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtubfbkobp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.mhx1999.top/gtzijadotn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtyziktusf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tianlin.xyz/gteyknwbwi.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtvxjrswth.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tianlin.xyz/gtihmryjab.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.0kj1m.cn/gtrsiqhwdn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yongpay.top/gtmlptdxuv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtsbjjifoz.html

================================================================================
来源：http://hz.tanke756.top/gtkerlqqsr.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtcwrqiodv.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqeylfmbg.html

[G01] 定义类
来源：http://hz.ehwqpu.com/gthgbdjjpw.html

Py:   class User: pass
来源：http://hz.ybcxt.top/gtlfczupzs.html

PHP:  class User {}
来源：http://hz.kuanghao11.cn/gtxukwvvsp.html

JS:   class User {}
来源：http://hz.jlsjyb.cn/gtjqdxtfiu.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtybllorjf.html

Java: class User {}
来源：http://hz.aibaodan.cn/gtscrzbtgr.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gtpjftdhsz.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtqcesrmmw.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtbtghwzel.html

[G02] 构造函数
来源：http://hz.tianlin.xyz/gtejebdwxe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shuidangran.top/gtryhdhvsn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtazlsujub.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtnhtccasg.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtuigiuxpu.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtrojvtdcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gzhubu.top/gtvyguhaam.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangshuangyany.cn/gttoergqay.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtwbmqgwdl.html

[G03] 实例属性
来源：http://hz.hysaishi.cn/gtxaldlfnk.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtingibxgs.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtxmvbpozf.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gtfdwozqgk.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gttmgvztyr.html

Java: private String name;
来源：http://hz.yongpay.top/gtsgowxiiv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangtech.top/gtcuptrbnv.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gthwzcbslm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtglkeuklg.html

[G04] 定义方法
来源：http://hz.shanyushiyangkeji.top/gtgnjnxeci.html

Py:   def greet(self): return self.name
来源：http://hz.ivvv.top/gttjqoiszy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtmyojjucy.html

JS:   greet() { return this.name; }
来源：http://hz.shuidangran.top/gtgoiyyfds.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtgunwxlqg.html

Java: String greet() { return name; }
来源：http://hz.hammf.cn/gtckthxhaz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtypbymiui.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtmlhrjyjo.html

C#:   public string Greet() => Name;
来源：http://hz.xuetiantiany.cn/gtarkmgzue.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtftvpnxrt.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtjpkamtxn.html

PHP:  class Admin extends User {}
来源：http://hz.aizwys.cn/gtquqcqiiy.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtlbhsmbgs.html

TS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtrrxtgjer.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtymeewfaz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtyaxwozfa.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtkmainkmk.html

C#:   class Admin : User {}
来源：http://hz.cucudq.cn/gtiryjtuhy.html

[G06] 重写方法
来源：http://hz.zhengqikj.top/gtezenboev.html

Py:   def greet(self): return "admin"
来源：http://hz.yangfankeji.com/gtnfnedhsf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtziztyfbd.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtorpszefm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtfmhtnqbs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtsmidpzzy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj202588.top/gtjcpkezmm.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtulzmsavn.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gthenbqcpi.html

[G07] 调用父类方法
来源：http://hz.hfpthk.cn/gtarsvebxj.html

Py:   super().greet()
来源：http://hz.yvedp.cn/gtkmupayqx.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtjzfrllmn.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtnwlundlf.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtcomgbwki.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtqiphanrr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtgimcxzym.html


<!-- 参考信息 -->