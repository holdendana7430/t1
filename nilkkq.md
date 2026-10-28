代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.xingfuxueyuan.xyz/gtrynjisui.html

JS:   items.join(",")
来源：http://hz.tanke756.top/gtnqtufyaq.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gteidvumbu.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gttfcbxnao.html

Go:   strings.Join(items, ",")
来源：http://hz.52xcode.cn/gtpgxvqwna.html

Ruby: items.join(",")
来源：http://hz.c1oappe.top/gtlnmtytxg.html

C#:   string.Join(",", items)
来源：http://hz.yueranfly.top/gtvfuskdjn.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtpwdwswja.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gtndpafudn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtadtasnkk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtrysndqml.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtnifxtijk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yangfankeji.com/gtylmjkrhp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gtrjdxltpa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shangyingyoupin.top/gtjeeycvev.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gttuahwhfd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.haohaochexian.top/gtzqnkroyc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtugdmqpaq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.kuanghao11.cn/gtfuikwqpm.html

JS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtyikiffxc.html

TS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtcixviicy.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtoggmower.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.haohaochexian.top/gttanwodmr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yueranfly.top/gteevmpxdk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtraaepdtp.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtrflafijs.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtqlqoruct.html

PHP:  strrev($s);
来源：http://hz.redwolf501.top/gthixwhbof.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gteszefwab.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtlhohsgom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuanzhike.top/gturjflglb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtrvtrpceo.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gtdypkblja.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtirxdytsi.html

[E12] 统计某字符出现次数
来源：http://hz.ppjwa.cn/gtazofwprn.html

Py:   s.count("a")
来源：http://hz.tanke756.top/gtijgswuda.html

PHP:  substr_count($s, "a");
来源：http://hz.shanyushiyangkeji.top/gtylznufzs.html

JS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtwuwjsjfv.html

TS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtalndibjz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hywenlv.cn/gtjxttmhjv.html

Go:   strings.Count(s, "a")
来源：http://hz.haohaochexian.top/gtyemjngjp.html

Ruby: s.count("a")
来源：http://hz.dashuyun.cn/gtumnpnvew.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jiagoushi.top/gtaaovkihf.html

[E13] 逐字符遍历
来源：http://hz.chenjidiqi.icu/gtiggbwwfv.html

Py:   for ch in s: print(ch)
来源：http://hz.zdqjudy.top/gttnmlshkn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.0kj1m.cn/gtahukwgvs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtpznggybb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtifguchjp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ivvv.top/gtczlscfev.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gzhubu.top/gtutvyefhh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtcfxofkch.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258888.top/gtpcoqwwhb.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtssvxcwfb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hfpthk.cn/gtqkriphnu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guowangkeji.top/gtaovbwoob.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gtfurnfmqq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtganhgevt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hfpthk.cn/gtarbdwmio.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtjngidqtw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gaohongyu789.top/gtvarrpdmv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtbqdiiwzd.html

[E15] HTML 转义 / 反转义
来源：http://hz.hysaishi.cn/gtvjutreqi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtuioqffeu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xingfuxueyuan.xyz/gtgcszxdnd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhengqikj.top/gtzpsgiwvb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtiyaftyor.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtxoeykpcw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtsgfrfomp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gteqtmmfbm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yvedp.cn/gtisphmhut.html

[E16] 数字千分位
来源：http://hz.gotoacloud.top/gthmpimwlo.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtwablcazq.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtsljmxqwg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtfxsvtjby.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtzhpjulgg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gtekjijntr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydjk.org.cn/gtbsvrpeid.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ywan-chungtsiang.top/gtwiaywjdx.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtamkejtdp.html

[E17] 首字母大写
来源：http://hz.zhoulong.xyz/gtjrxfdqty.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinqigufen.top/gtqtqoonfm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.bjfxy.top/gtszvrpkzx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtlkcxfzvg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtpnofvwwk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.haohaochexian.top/gtpwxntoor.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zycfv.cn/gttqrtqpxj.html

Ruby: s.capitalize
来源：http://hz.guowangkeji.top/gtqtniaorl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gtgygkqyxt.html

[E18] 模板占位符替换
来源：http://hz.jqgfzy.top/gtkwwhdnla.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhongyouzk.top/gtbwcrkfsb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gthzrbjkyo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtfwipnoua.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtlyidvmgu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.0kj1m.cn/gtbucgnsrf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtznlvnjpv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jiagoushi.top/gtnvdmiaup.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.guowangkeji.top/gtkqrzluzy.html

[E19] 多行文本按行拆分
来源：http://hz.xuetiantiany.cn/gtgxpxngvn.html

Py:   s.splitlines()
来源：http://hz.hywenlv.cn/gttsibqpdn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gtmwwwhemv.html

JS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtopjvpbaj.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtmsqymddd.html

Java: s.lines().toList()
来源：http://hz.yueranfly.top/gtudeearnc.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258888.top/gtwjzixpke.html

Ruby: s.lines
来源：http://hz.jinghuilouyu.cn/gtsfgkedpv.html

C#:   s.Split('\n')
来源：http://hz.gotoacloud.top/gtguiftjys.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtfpwjpbwu.html

Py:   if not s:
来源：http://hz.hnqzz.top/gtksnswnao.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xylfe.cn/gtkvwzssoj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.iojbl.cn/gttohztdhp.html

TS:   if (s === "") {}
来源：http://hz.c1oappe.top/gtpuhtbnmi.html

Java: if (s.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtrlnnacpl.html

Go:   if s == "" {}
来源：http://hz.jinyuanbaomall.cn/gtnumllryu.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtvtiawgam.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenjidiqi.icu/gtmolleqtx.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtzaetqgrx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nwbrower.top/gtfgorbezu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.redwolf501.top/gtevklelxg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtueehoakl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtklnzdhfg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtnujejruy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gtrumpsttb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtqsurkemn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtivwvtebv.html

[E22] 字节长度与字符长度
来源：http://hz.hfpthk.cn/gtwjjkfzfw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gtflgwbmmv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtycuzchrd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zycfv.cn/gthsbrfegz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtmkkrsryh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhaomingkeji.xyz/gtouomwghn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtqezemnyv.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhongyouzk.top/gthyqaaahd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtifxrunpo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlyhbyifi.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtpcgtsahf.html

================================================================================
来源：http://hz.c1oappe.top/gtgclsqqpk.html

[F01] 读取整个文件
来源：http://hz.xinyue.icu/gtuasvgrmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.vqdsnc.cn/gtmpvilksq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtcbiphnrw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtukoibwdz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtljyzeryc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtbkulvrmw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gtdvqdrium.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtpcwdxost.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.vqdsnc.cn/gtailyvvej.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtxlzsgpif.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxinkj.top/gtvkabczsa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hfpthk.cn/gtgeuwkesx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtovvbagth.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtymayujej.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sweek.top/gtngdrbbhk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.0kj1m.cn/gtqnnqiqdj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fengsongda.top/gtqoisecwq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtsamrvrvr.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtbyyijzig.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guowangkeji.top/gtxjjgdstq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtjgnafahj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtvjfqbxqu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtldarmnuu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gtgqrtmxdu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtzjjtuotu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.iojbl.cn/gtndslpept.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtlwwhozed.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtanvhjgty.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.kuanghao11.cn/gtxtbvqahg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhaomingkeji.xyz/gtgxwaczul.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtlruukwoy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtbaqoitun.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtgwurewqv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj202588.top/gtqbbrmzqz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gtojoipntr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxinkj.top/gtoofbdxdr.html

[F05] 判断文件或目录是否存在
来源：http://hz.yonumen.top/gtdvuxqugs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtpcclwckz.html

PHP:  file_exists("a.txt");
来源：http://hz.zdqjudy.top/gtwwjrmjsy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtgxxtcxvk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtgpnrbnsi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtqqlzgubt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.meibo888.top/gtwtnxfgkp.html

Ruby: File.exist?("a.txt")
来源：http://hz.sufxvd.cn/gtzinjritu.html

C#:   File.Exists("a.txt")
来源：http://hz.ydzc1.top/gtwllerepd.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtawupeyfv.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gthhvewsef.html

PHP:  unlink("a.txt");
来源：http://hz.guannengcc.top/gthotillds.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtshaegbpy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtxodlrxek.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtsbvctunc.html

Go:   os.Remove("a.txt")
来源：http://hz.zhongyouzk.top/gtvtdkxywz.html

Ruby: File.delete("a.txt")
来源：http://hz.shangyingyoupin.top/gtbsjbvljq.html

C#:   File.Delete("a.txt");
来源：http://hz.sufxvd.cn/gtsclbhhas.html

[F07] 创建目录（含多级）
来源：http://hz.zhiwuduotai.top/gtbkefruxr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xylfe.cn/gtylcergcu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shuidangran.top/gtpqylrtvs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gthvaakylc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuanzhike.top/gtwqttelnb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtjldpfoau.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.smart0.xyz/gtclmiqwfk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pycfn.com/gtbuunozmc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtmxrywxzq.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gtiztncomv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.haohaochexian.top/gtptwggnej.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guannengcc.top/gtgxarwtxl.html

JS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gttdodbsdr.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtxwkiqsaj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtxbjetjop.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.iojbl.cn/gtilpywvkf.html

Ruby: Dir.children("dir")
来源：http://hz.jianghu66.top/gtcmpwmixj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cashguo.top/gtoipftibp.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gtiullaspb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.birdmap.top/gtqhwwriek.html

PHP:  filesize("a.txt");
来源：http://hz.ppjwa.cn/gtvmjukobp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtahhziqlq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtazsvgufn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtrqqjdohw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gthzicotjt.html

Ruby: File.size("a.txt")
来源：http://hz.guannengcc.top/gtapdpobxn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.9152youxi.cn/gtofrolids.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gtwwldrbjb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmdgxwyxk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtjozovxko.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtyszevsca.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtbxxqhvto.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuanzhike.top/gtzssjnfez.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtdvoxocul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtjzqzbdod.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtpqxsddjn.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangkeji.top/gtagomowoj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtyfxghffr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtitekkhst.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtaqyoxclr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtirvrnrvu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gotoacloud.top/gtkkgtwagh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtdmtxniue.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtxhdjxejd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hammf.cn/gtqyymtdxd.html

[F12] CSV 读写
来源：http://hz.chenjidiqi.icu/gtimzlqcws.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtrrecbknl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.vqdsnc.cn/gtnqzdodrx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtlkvklqox.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtcostcadi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangtech.top/gtlamdttli.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtmigtysmb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gogol.net.cn/gtjdwgyspk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jyoumei.cn/gtuyjmjaqw.html

================================================================================
来源：http://hz.ehwqpu.com/gthfacslyf.html

G. 面向对象
来源：http://hz.ybcxt.top/gtqteiokjj.html

================================================================================
来源：http://hz.jinqigufen.top/gtccmpcufu.html

[G01] 定义类
来源：http://hz.yangfankeji.com/gtvsqrrfhq.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gteyznlhjo.html

PHP:  class User {}
来源：http://hz.yongpay.top/gtqphrzzrd.html

JS:   class User {}
来源：http://hz.ivvv.top/gthpgczbye.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtqlnsqyae.html

Java: class User {}
来源：http://hz.meibo888.top/gtneewppml.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtbiokuhlg.html

Ruby: class User; end
来源：http://hz.birdmap.top/gtveluolrx.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gtdxhofsav.html

[G02] 构造函数
来源：http://hz.yongpay.top/gtzssymvya.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gttgunloth.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yonumen.top/gtabbxfkmw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtvbpdohlc.html

TS:   constructor(public name: string) {}
来源：http://hz.52xcode.cn/gtedpcihrr.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtbwnwyorp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jyoumei.cn/gteinbebzt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtwoutzowr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuanzhike.top/gtbndjydjj.html

[G03] 实例属性
来源：http://hz.xylfe.cn/gtygttvcmp.html

Py:   self.name = "x"
来源：http://hz.cheryme.top/gtklqjaayx.html

PHP:  public string $name = "x";
来源：http://hz.hywenlv.cn/gtfvfeqbvc.html

JS:   this.name = "x";
来源：http://hz.jinqigufen.top/gtullkngtl.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtmdqgmkbz.html

Java: private String name;
来源：http://hz.tanke756.top/gtgqfuymlc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtucqwepml.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gtfodailfj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtghbehogn.html

[G04] 定义方法
来源：http://hz.hysaishi.cn/gtkzvzkims.html

Py:   def greet(self): return self.name
来源：http://hz.chenzaomai.com/gtqpjdvaqb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtwunwyzmj.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtkjpguaej.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtslmlthan.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtmlnskkqq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gthyabstwq.html

Ruby: def greet; @name; end
来源：http://hz.aizwys.cn/gtbdsfxrwh.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gtkrxtjdbw.html

[G05] 继承
来源：http://hz.yvedp.cn/gtgheyenet.html

Py:   class Admin(User): pass
来源：http://hz.shangyingyoupin.top/gtknzdsltl.html

PHP:  class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtofarvusg.html

JS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtjzmtvlhj.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtyrfngtdf.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gteepiomap.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.meibo888.top/gtspfzuqwb.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtrfmuablt.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtztepbynq.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtptmtcwfw.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtctbwuzeq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtirjrkxwa.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtsnijliku.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtzxxfydza.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtvyfdlsad.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtfzdhuyri.html

Ruby: def greet; "admin"; end
来源：http://hz.birdmap.top/gtwsofrqyt.html


<!-- 参考信息 -->