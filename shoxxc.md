代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xylfe.cn/gtpqcquojs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.andypj.xyz/gtgkohtyll.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtxkpqqqog.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtqjalbdbq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtpmszzaou.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hysaishi.cn/gtaxxvxfiy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yanxiufei.cn/gtuzccwimc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zdqjudy.top/gtzpoanuhf.html

[E06] 替换子串
来源：http://hz.xuanzx.com/gtbfkdwliq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pycfn.com/gtvxpymbnq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258.top/gtkddeibdn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtqwxhjkpi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtuvgyybsj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtqduvqlvi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.iojbl.cn/gtoqpmwyuj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtalrjknzx.html

C#:   s.Replace("a", "b")
来源：http://hz.smart0.xyz/gtpwsttmwz.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gthfrfqwlc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gtaatoowro.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fzhhl.top/gtoheftbjk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtjecvzbdm.html

TS:   s.split(",")
来源：http://hz.hammf.cn/gtubecrpvp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtbvhscfep.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj202588.top/gtmqtedkun.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gtubwngmsx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ehwqpu.com/gtemypdtnv.html

[E08] 数组按分隔符合并
来源：http://hz.jinyuanbaomall.cn/gthewdirzw.html

Py:   ",".join(items)
来源：http://hz.shuidangran.top/gthuageblv.html

PHP:  implode(",", $items);
来源：http://hz.gaohongyu789.top/gtcdlybuyo.html

JS:   items.join(",")
来源：http://hz.andypj.xyz/gtckazfecc.html

TS:   items.join(",")
来源：http://hz.jyoumei.cn/gttetdpgot.html

Java: String.join(",", items)
来源：http://hz.jinghuilouyu.cn/gtcutdiykg.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangtech.top/gtuuimelww.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtzfgrvatu.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtypqieppk.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gteynyagoz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtrheminft.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.smart0.xyz/gtnutxjgcp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtoufbuljb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtwqdfmurf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jlsjyb.cn/gtdkjgsywf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtnfgaikbl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.bjfxy.top/gttevikddi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.haohaochexian.top/gtklfvgypf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.haohaochexian.top/gttpswsnlw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhixingplan.top/gtbgbavjfc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenlongwang.top/gtzutmhnud.html

JS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtvvmjybhq.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtbeqfavua.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtvgoifmrs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hfpthk.cn/gtabxdsakb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhengqikj.top/gtmdqghrue.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangkeji.top/gteqkjpkse.html

[E11] 反转字符串
来源：http://hz.jinqigfzy.top/gtomgwllsy.html

Py:   s[::-1]
来源：http://hz.iojbl.cn/gtzawkskly.html

PHP:  strrev($s);
来源：http://hz.sufxvd.cn/gttpqfggmb.html

JS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtrdobifjc.html

TS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtvhswxpth.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnxiangtu.top/gtjqsjwjor.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenzaomai.com/gtkcizzjgp.html

Ruby: s.reverse
来源：http://hz.ydzc1.top/gtkbjgrrpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtmotcbufv.html

[E12] 统计某字符出现次数
来源：http://hz.dianchejie.cn/gtcfmxvfuv.html

Py:   s.count("a")
来源：http://hz.sxryk.cn/gtvswztbyt.html

PHP:  substr_count($s, "a");
来源：http://hz.yj20258.top/gtlysoowxw.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtfhuysatj.html

TS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtxtivnbnk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yvedp.cn/gtjhxoeibp.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtvpdwiwpc.html

Ruby: s.count("a")
来源：http://hz.zhijiandao.cn/gtpscradtd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gterthiigk.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtssyissnp.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtrvaaddtz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhixingplan.top/gtkeefwogi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtdwwozkbv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtkeqpefwf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hysaishi.cn/gtdknbqtny.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cucudq.cn/gtugihnpvg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtllomgjsn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.52xcode.cn/gtrqdjlcql.html

[E14] URL 编码与 Base64
来源：http://hz.ybcxt.top/gtwejpnupr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtcqgxahby.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhixingplan.top/gtochxszqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sysykeji.top/gthbjkvzzw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydjk.org.cn/gtjmtgcpcu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tianlin.xyz/gtruguvxcz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydjk.org.cn/gtgsbdvcbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gogol.net.cn/gtfxfvjpcr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.vqdsnc.cn/gtulrdcfiu.html

[E15] HTML 转义 / 反转义
来源：http://hz.zdqjudy.top/gtrsbkoisb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhijiandao.cn/gtztmkrsxp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hywenlv.cn/gtiytvsftp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hfpthk.cn/gtujbiivog.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jiagoushi.top/gtxdioyici.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aizwys.cn/gtcxoxyadt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtgkzvesae.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtpgyhpfkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuetiantiany.cn/gtxtewdewu.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gttaipdwou.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtiluyhuse.html

PHP:  number_format(1234567);
来源：http://hz.52xcode.cn/gtpmbnaxbb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtfjsqcubx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtjzqlmave.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gtcizenmoa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxinkj.top/gtpefmzddr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gticfrjqze.html

C#:   1234567.ToString("N0")
来源：http://hz.nwbrower.top/gtpmnowpdb.html

[E17] 首字母大写
来源：http://hz.9152youxi.cn/gtqzpmwiqa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gtjqhfzill.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtqaqdwhvp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtmsdvflsk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtzbffjvkz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtjevhfefg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gtfalgvoik.html

Ruby: s.capitalize
来源：http://hz.feifeiyinyue.top/gtamsgjbfc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtbxvijddp.html

[E18] 模板占位符替换
来源：http://hz.zycfv.cn/gtxxmxwhev.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtfdsqokdv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gtdwqwjlnf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtsgawfacb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtgxjooytv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydzc1.top/gtzyfwzgpt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtrojxagbl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtpdesrwlr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtrcyonwfp.html

[E19] 多行文本按行拆分
来源：http://hz.pycfn.com/gtgbrdnvdu.html

Py:   s.splitlines()
来源：http://hz.andypj.xyz/gtdfccxysu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtozfefyje.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtuilnmsnm.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtalyhuaax.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gtfomrzxra.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhaomingkeji.xyz/gtqdsiuqjw.html

Ruby: s.lines
来源：http://hz.xuetiantiany.cn/gtugkgnznb.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gthofigdgx.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtzviuzmrx.html

Py:   if not s:
来源：http://hz.yj20258888.top/gthtbbvqqn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shuidangran.top/gtapuyhfbb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtesrdixhd.html

TS:   if (s === "") {}
来源：http://hz.yuanzhike.top/gtgxxqmuia.html

Java: if (s.isEmpty()) {}
来源：http://hz.yongpay.top/gtbcmshkip.html

Go:   if s == "" {}
来源：http://hz.hysaishi.cn/gtilffgdww.html

Ruby: if s.empty?
来源：http://hz.guannengcc.top/gtxtyllcgb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gaohongyu789.top/gtypgxgczs.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gthruekkgj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yvedp.cn/gtxejnytpf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtfhsilnov.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtgewicmit.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtyspvupjo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtcefqlutp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jlsjyb.cn/gtlrcqeksx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xinyue.icu/gtflfxicfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gtenndpmtz.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gtpljruqms.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydzc1.top/gtvbjelcoj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtobwpbjbs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtqhphcijz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtzwpuihwb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtotxyywmu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jlsjyb.cn/gtswtzzzbe.html

Ruby: s.bytesize;  s.length
来源：http://hz.ybcxt.top/gthomubdfd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gteqbwycbw.html

================================================================================
来源：http://hz.aibaodan.cn/gtkndnizsi.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gtwgxqqfeh.html

================================================================================
来源：http://hz.yongpay.top/gtvniknlji.html

[F01] 读取整个文件
来源：http://hz.0kj1m.cn/gteantkvif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jiagoushi.top/gtboozxhkp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jianghu66.top/gtcaeobgsq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtdvnywlwu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hammf.cn/gtiopdfzvk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtdrnyvifp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigfzy.top/gtrfqvjvzo.html

Ruby: File.read("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtgscnsgre.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuanzx.com/gtbgxcnrwg.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtkdkmqobh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydjk.org.cn/gtassocxju.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtucsojdae.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtnaetmaty.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gthqgxmdzo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtdguudmne.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhijiandao.cn/gtqaopekex.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nanxuanxn.top/gttcgosfkp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtsxgpjaqs.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtunojookn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxinkj.top/gtwohcttmf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtcmnormjj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtefvzbslw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtxojgstbx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtiqhamcmp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtuhkkricr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtzxamqjgp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fzhhl.top/gtrhxlsgbg.html

[F04] 追加写入文件
来源：http://hz.xuetiantiany.cn/gthuvdsigc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtlyuglsxa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gzhubu.top/gtmesorcyy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtffhpxene.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtkjosjdha.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jyoumei.cn/gtnujbywrl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gtpwrqlpmq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtukafnszq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dianchejie.cn/gtmmavwslj.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gttnaugxrl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenzaomai.com/gtyotqfekw.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtydtugltb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtaddqhgav.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gtftqpeozd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtcgesyxkd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtgekbqfpk.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtxppyvprn.html

C#:   File.Exists("a.txt")
来源：http://hz.tian-w.cn/gtcphnamcq.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gteqvnbdbs.html

Py:   os.remove("a.txt")
来源：http://hz.redwolf501.top/gtxylwptlc.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtwurkcesx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtarjptidb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtgszpjcgb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtpixbgrtd.html

Go:   os.Remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtbwbdwezo.html

Ruby: File.delete("a.txt")
来源：http://hz.hfpthk.cn/gtjslyibxw.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gttztdmtnt.html

[F07] 创建目录（含多级）
来源：http://hz.meibo888.top/gtdrjnddzw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gthpoqnesl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtszaoqdbz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtrdnftkyc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtagfmwfnj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.andypj.xyz/gtqgmqwfie.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtmadnpuzn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhoulong.xyz/gtixrxjisd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aibaodan.cn/gtgdiinvsl.html

[F08] 遍历目录
来源：http://hz.shanyushiyangkeji.top/gtgjezxgle.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gtyqadbgyh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtzbbenzig.html

JS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtpoxtdaav.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtdpcsjuuc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtyorgjaqo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtcpeukhly.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtgzmacdre.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtnlalotxy.html

[F09] 获取文件大小
来源：http://hz.zhaomingkeji.xyz/gthlehxhfi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenlongwang.top/gtvprdztdz.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtaecbowfd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtbmsudcdu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtgsqkzjvi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtmisitbho.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.andypj.xyz/gtfbjujjhl.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtbcqjrtxv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258.top/gttmpdmrys.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtktaggksx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtiixqopag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.vqdsnc.cn/gtkxgnqtqb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtkjmktkxi.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gttsrrmmid.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yvedp.cn/gtxhfaqxnv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.birdmap.top/gtfnxuelqg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtcvkznyue.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gtsilryote.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtsmwrrssm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtlsdznjwf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtnymzxaem.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtnofjeyhu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtdzjgvmlf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtmfqyepeg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yonumen.top/gtdlocbwct.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gttqepdtyn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtagzltonb.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtlnbsizyw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtefnfoewm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtixmfkami.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cucudq.cn/gtmqvnqbzk.html

TS:   // 同上
来源：http://hz.316326.xyz/gthuarhola.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258.top/gtgzfkgagm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gaohongyu789.top/gtmeakeivc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtqakexpdc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sxryk.cn/gthbwhvkng.html

================================================================================
来源：http://hz.hammf.cn/gtjccighku.html

G. 面向对象
来源：http://hz.daxiang520.top/gtozooierb.html

================================================================================
来源：http://hz.svipenyu.cn/gtaodoulpk.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gtmgamxnzd.html

Py:   class User: pass
来源：http://hz.zhixingplan.top/gtknjoucsk.html

PHP:  class User {}
来源：http://hz.jinghuilouyu.cn/gtxmcisjgy.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtrhpmdqnp.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtadoysils.html

Java: class User {}
来源：http://hz.zhoulong.xyz/gttugzeeek.html

Go:   type User struct { Name string }
来源：http://hz.cheryme.top/gtkxjmqzxl.html

Ruby: class User; end
来源：http://hz.shangyingyoupin.top/gttnqaharu.html

C#:   class User {}
来源：http://hz.yongpay.top/gtollmoywf.html

[G02] 构造函数
来源：http://hz.shzxlz.cn/gtlmakmdwb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydzc1.top/gtpvtjqapa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xylfe.cn/gtbsncgaiu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtlkxrmfbu.html

TS:   constructor(public name: string) {}
来源：http://hz.xuanzx.com/gtuvnxyycr.html

Java: User(String name) { this.name = name; }
来源：http://hz.tanke756.top/gtqlpapcko.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtbirqbmpc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.iojbl.cn/gtgwtnisxd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shangyingyoupin.top/gtjaiihpwy.html

[G03] 实例属性
来源：http://hz.zycfv.cn/gtfbhcgaaa.html

Py:   self.name = "x"
来源：http://hz.guannengcc.top/gtxvnlcjhq.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtciuolwln.html

JS:   this.name = "x";
来源：http://hz.chenzaomai.com/gtqguwssgk.html

TS:   name: string = "x";
来源：http://hz.hnxiangtu.top/gtxbpsbwkf.html

Java: private String name;
来源：http://hz.meibo888.top/gtbdomcjgp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnqzz.top/gtcjoinvxa.html


<!-- 参考信息 -->