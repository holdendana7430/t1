代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtkqzewrex.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gtzhbknjtd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dianchejie.cn/gtspjutcxl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgfzy.top/gtexwyxzir.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtlrawipdf.html

[E11] 反转字符串
来源：http://hz.cqqwz.cn/gtpvsjintj.html

Py:   s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtbkmnoday.html

PHP:  strrev($s);
来源：http://hz.zhijiandao.cn/gtptvrlacw.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtyvvrpplh.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtrozvgvif.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aibaodan.cn/gtkzizribd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aibaodan.cn/gttflkrxzy.html

Ruby: s.reverse
来源：http://hz.feifeiyinyue.top/gtxkhbfcej.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtsjzcmebb.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtcxdxuqmg.html

Py:   s.count("a")
来源：http://hz.hysaishi.cn/gtonncaqyp.html

PHP:  substr_count($s, "a");
来源：http://hz.pengpengdd.cyou/gtuchqsaht.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gthoytjjgz.html

TS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtuxhrnhod.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhaomingkeji.xyz/gtvlcqdtoz.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gtovbwlafo.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtzdtcaxis.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xinyue.icu/gtigujeemn.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtztyipobl.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gtzughcmiu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenlongwang.top/gtdgptjwyw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtdwnwjfol.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gthjrtiofz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cdnleiting.top/gtdtlwhmxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtudpezakh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhiwuduotai.top/gtvckqzlwg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtbfxbaiwd.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtmaucbdqq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zdqjudy.top/gtyvvhspiz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhoulong.xyz/gthwnsnhzd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gtlucwzqva.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtsmhjqpyf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hywenlv.cn/gtmqyuwbqe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtrpzdcogc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yueranfly.top/gtdlmcjfff.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gtkbpdzuvb.html

[E15] HTML 转义 / 反转义
来源：http://hz.jiagoushi.top/gtypehidqp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yonumen.top/gtyjunumdn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangtech.top/gtujtgtiae.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hywenlv.cn/gtzeqsdvzx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gogol.net.cn/gtlnbwyekj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258888.top/gtfzwgesse.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhiwuduotai.top/gtavzzqumj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtkqigvoyp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ybcxt.top/gtwpkzydpu.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gtkdjioral.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtnyjiqzej.html

PHP:  number_format(1234567);
来源：http://hz.bjfxy.top/gtgqqrujtu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtnuubeayj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtrjzmycvr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hysaishi.cn/gtnyjuudbi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gttihvldbv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gtmebbuctr.html

C#:   1234567.ToString("N0")
来源：http://hz.yuxming.cn/gtxirzljxe.html

[E17] 首字母大写
来源：http://hz.xuetiantiany.cn/gtiwsmyinl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtqbzhnnpa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtccdtcjrx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtqkbyeumd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtsijklaam.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yvedp.cn/gtlzycnolk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gtevxwfaaq.html

Ruby: s.capitalize
来源：http://hz.hywenlv.cn/gtmojkliqf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhongyouzk.top/gtgweqpirt.html

[E18] 模板占位符替换
来源：http://hz.sweek.top/gtavkrchek.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtxobnqled.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xinyue.icu/gtqnidtkai.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtnvipwtll.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtkqrtseyq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sysykeji.top/gtrwtyniiz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jiagoushi.top/gtkooldicv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gtwmsskgrj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtjkneymqe.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtycscpula.html

Py:   s.splitlines()
来源：http://hz.yuanzhike.top/gtcsqhfwrv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtplqsvfqz.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtyzcbgjkz.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtvlpulrlt.html

Java: s.lines().toList()
来源：http://hz.ydjk.org.cn/gtlhnwhpff.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj202588.top/gtkafhjdqc.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtkvjfpgkl.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtawpvyemd.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtoezeonsg.html

Py:   if not s:
来源：http://hz.hywenlv.cn/gtwhadhnpq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnxiangtu.top/gtumssbjvy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xylfe.cn/gtfiadhlob.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtqwxdcjgp.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gtualngqwx.html

Go:   if s == "" {}
来源：http://hz.cashguo.top/gtamktbfkk.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtrijnurvb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtohwqiwfb.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gtsbrwslsg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yangfankeji.com/gtlebglusz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhengqikj.top/gtgcexxabo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtsnvyvixc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtknjblbko.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtmzubvxwj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gtegrpafrc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gogol.net.cn/gtdmcwcdbm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtspssught.html

[E22] 字节长度与字符长度
来源：http://hz.kuanghao11.cn/gtlcyqoyjp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtmtyrqmdj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtsteoogin.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtvzwwwoma.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtchnlccky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gtyytdlclz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.bjfxy.top/gtwkuiulmo.html

Ruby: s.bytesize;  s.length
来源：http://hz.9152youxi.cn/gtdbphrnqk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtgptknjug.html

================================================================================
来源：http://hz.zhixingplan.top/gtvuaynpnx.html

F. 文件与目录
来源：http://hz.dashuyun.cn/gtzspqurma.html

================================================================================
来源：http://hz.mhx1999.top/gtgjvobscw.html

[F01] 读取整个文件
来源：http://hz.yuxming.cn/gtvfzncuzg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtnduufxhh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gtedhjbbta.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gtaosaoedv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtbocithqh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtlzkeaofg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.kuanghao11.cn/gtiaiodtvj.html

Ruby: File.read("a.txt")
来源：http://hz.jlsjyb.cn/gtnfduxfrn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pengpengdd.cyou/gtmidplgvr.html

[F02] 逐行读取文件
来源：http://hz.xingfuxueyuan.xyz/gtbtxlaguj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtifvgojoj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangshuangyany.cn/gtzojxvges.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtsbnmrbxc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtvsprfjmm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtxlmxtdkh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtcffvshjd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtrmmvcqim.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tanke756.top/gtujkcsqqz.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258888.top/gtpxxhxfrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cdnleiting.top/gtfjcbzdnu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtzuxjkwna.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtvmvhadkf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtleozpleu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtwvpmgxpl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yonumen.top/gtwtjwvhbb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aizwys.cn/gtiakbkzpg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtybvqbbvq.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gthffusrrm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtrffjgipx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtqnyykgqm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtoriqavca.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtvcbytmhn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhaomingkeji.xyz/gtwerikuva.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gtuzmpjfgv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fengsongda.top/gtrzwyczkw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ppjwa.cn/gtqbvctqqd.html

[F05] 判断文件或目录是否存在
来源：http://hz.gzhubu.top/gtanwnenzu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtnxhtehix.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtrqxomehn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtfvybjtkt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtcvafwosr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtifzemvua.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xziqi.cn/gtklijcwum.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtlnizbxng.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gtkxxbnnfp.html

[F06] 删除文件
来源：http://hz.316326.xyz/gtkaouatpj.html

Py:   os.remove("a.txt")
来源：http://hz.smart0.xyz/gtoxrlqspi.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtneonwjwb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtjyzwjwgf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtnlibtrdo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtwdzpcmde.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtcjqxaotg.html

Ruby: File.delete("a.txt")
来源：http://hz.ydzc1.top/gtsjmyfnzs.html

C#:   File.Delete("a.txt");
来源：http://hz.yueranfly.top/gtksxcvago.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtccgpueyx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydjk.org.cn/gtctotpikp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtmypnwxlp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtagvqvocm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gttgqtlgpm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtkwjmfeyv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtkoanpyxv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydzc1.top/gtynvhxsco.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guannengcc.top/gtunqhyvcl.html

[F08] 遍历目录
来源：http://hz.yuanzhike.top/gtrmkdypvo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nanxinkj.top/gthdxfboyr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gaohongyu789.top/gtyiamhpfz.html

JS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtqywyhjii.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtdpxhbafz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gtgkknairf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtgmquvugk.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gthyvcvbgf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtvbjunywq.html

[F09] 获取文件大小
来源：http://hz.52xcode.cn/gtohwoejfl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xziqi.cn/gtvjyywias.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtfgoeezad.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtgnimbhez.html

TS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtuptqswex.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtikpomiyg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daria6918.cn/gteyplcmeg.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gttgcaejgd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtxprthylu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtchlfmrhg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtvitjtksi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydzc1.top/gtnsoxpeyw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtpzrzqavt.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258.top/gtkxhdsbrx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuanzx.com/gtprwtupad.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtwpyagobi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gthlmjfadt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtwynhblat.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtbaxytiqd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtrojgbglo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gtsydbwehi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtnzwojuav.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtbrlkqjud.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhixingplan.top/gtbtzgthcq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtzxhnlrvl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtnefeqjak.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gzhubu.top/gtvsmgdhzy.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtaegvrlav.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gtftkcjbah.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtvqzgsvma.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtsxsjrhcx.html

TS:   // 同上
来源：http://hz.fzhhl.top/gtzkmxmcva.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtgediutoq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gtjjjahgdz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxuanxn.top/gtxkrnlomb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtadsjjhwq.html

================================================================================
来源：http://hz.birdmap.top/gtvxotawhh.html

G. 面向对象
来源：http://hz.jinyuanbaomall.cn/gtbyfxqcax.html

================================================================================
来源：http://hz.hywenlv.cn/gtrttjcoft.html

[G01] 定义类
来源：http://hz.cashguo.top/gtphqtpbck.html

Py:   class User: pass
来源：http://hz.jqgufenzy.top/gtdzoiimwa.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtlegqurvf.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtocspkrci.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gtltcizbqh.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtcwzjxuoj.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtrymzxpjq.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtjsgpobpc.html

C#:   class User {}
来源：http://hz.chenlongwang.top/gtjlukwdfp.html

[G02] 构造函数
来源：http://hz.smart0.xyz/gtjsawaasj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gtkpbsqjcx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tian-w.cn/gtiactkiaj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtjyuaymhk.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gthvaxkxmb.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangdashe.top/gtapljixvz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dianchejie.cn/gtmrmkaqus.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gtguhbsnfn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtefgkmbkm.html

[G03] 实例属性
来源：http://hz.yonumen.top/gtrbgbkndq.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtkehwjlcl.html

PHP:  public string $name = "x";
来源：http://hz.yvedp.cn/gtrwhaojyn.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtkjxakefm.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gtrdnbhtwa.html

Java: private String name;
来源：http://hz.ivvv.top/gtioavvdbs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtwfrrtnzp.html

Ruby: @name = "x"
来源：http://hz.dashuyun.cn/gtwjcpzbit.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xingfuxueyuan.xyz/gtvsrpohjy.html

[G04] 定义方法
来源：http://hz.smart0.xyz/gtmvcjtmja.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gttkzzhrei.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtpdrpqywy.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtugbdsdfs.html

TS:   greet(): string { return this.name; }
来源：http://hz.tanke756.top/gtzridafzs.html

Java: String greet() { return name; }
来源：http://hz.xylfe.cn/gtejqgrzcr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtjzvbzehc.html

Ruby: def greet; @name; end
来源：http://hz.sysykeji.top/gttjgwjfzj.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gtxoonucik.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtxoqmnbyv.html

Py:   class Admin(User): pass
来源：http://hz.chenlongwang.top/gtoahlprgg.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtgdywbsjn.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtpkncdolr.html

TS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtmigdipoy.html

Java: class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtwehyfwnn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.havefunace.top/gtltbjrfhb.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtmpmfwgnb.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtgbeofbyx.html

[G06] 重写方法
来源：http://hz.yangfankeji.com/gtdukkptbj.html

Py:   def greet(self): return "admin"
来源：http://hz.zhoulong.xyz/gtkcfopmvy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtetiwxfgw.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtgyzmkdug.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gteiknjhoa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtawnlkqfv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtippjryih.html

Ruby: def greet; "admin"; end
来源：http://hz.dashuyun.cn/gtibmyiwot.html

C#:   public override string Greet() => "admin";
来源：http://hz.sxryk.cn/gtnpxvuscs.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtswulijht.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtybxhkhgi.html

PHP:  parent::greet();
来源：http://hz.xuetiantiany.cn/gtejrsklha.html

JS:   super.greet();
来源：http://hz.daxiang520.top/gtbidkwqps.html

TS:   super.greet();
来源：http://hz.yongpay.top/gthjvfkftf.html

Java: super.greet();
来源：http://hz.birdmap.top/gtlpvjhzsu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.9152youxi.cn/gtuqpefcdd.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtlhapecvj.html

C#:   base.Greet();
来源：http://hz.wangshuangyany.cn/gtpdzupvdn.html

[G08] 静态方法与属性
来源：http://hz.zhixingplan.top/gtmrxxsykr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.meibo888.top/gtlkoacxfh.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtikspitte.html

JS:   static f() {}
来源：http://hz.jyoumei.cn/gtzrzfwbmh.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gtpcwcjkzr.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gtzljyzqkm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtdwqlfqjg.html

Ruby: def self.f; end
来源：http://hz.zdqjudy.top/gtrujxzvrr.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtzplqhncd.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtgssqnell.html


<!-- 参考信息 -->