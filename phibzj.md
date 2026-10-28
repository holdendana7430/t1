代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.jqgufenzy.top/gtqaqmjwgx.html

[E07] 按分隔符拆分
来源：http://hz.nanxuanxn.top/gtuvnsofmu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ywan-chungtsiang.top/gteyrzlyzc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtddqytmbj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cashguo.top/gteqtmezxw.html

TS:   s.split(",")
来源：http://hz.chenlongwang.top/gthqiltvid.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shangyingyoupin.top/gtgssxydxr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydjk.org.cn/gtilzeoaft.html

Ruby: s.split(",");  s.split
来源：http://hz.yueranfly.top/gtdzghvjtv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.0kj1m.cn/gtnxqffqtq.html

[E08] 数组按分隔符合并
来源：http://hz.zhengqikj.top/gtaopgxfcu.html

Py:   ",".join(items)
来源：http://hz.dianchejie.cn/gtkaxvqufa.html

PHP:  implode(",", $items);
来源：http://hz.mhx1999.top/gtynxmalsx.html

JS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtkcflvbpf.html

TS:   items.join(",")
来源：http://hz.quarkkingdee.top/gttwlwhfas.html

Java: String.join(",", items)
来源：http://hz.jyoumei.cn/gthecclghr.html

Go:   strings.Join(items, ",")
来源：http://hz.zhongyouzk.top/gttniagbkl.html

Ruby: items.join(",")
来源：http://hz.hongshengwenyu.top/gtcybtheiq.html

C#:   string.Join(",", items)
来源：http://hz.ehwqpu.com/gtzwsbpcmk.html

[E09] 去除所有空白字符
来源：http://hz.aizwys.cn/gtsyvxtjvj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nwbrower.top/gtlefsylpg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtxinfvfxq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sufxvd.cn/gtnguhhyrr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtsrswrcug.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cheryme.top/gtakfyzrnh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtfnoplsko.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.meibo888.top/gtnargipgt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dianchejie.cn/gtbkltgjcv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.quarkkingdee.top/gtutbnerad.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydzc1.top/gtchdelfgz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.9152youxi.cn/gtzgyodoph.html

JS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtukeqclnw.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gteqnybzqf.html

Java: String.format("%03d", 7)
来源：http://hz.nanxinkj.top/gtdjvpbgfl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sufxvd.cn/gtfohurahl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtvlnhfing.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigufen.top/gtaeouqlff.html

[E11] 反转字符串
来源：http://hz.havefunace.top/gtjgevqsoo.html

Py:   s[::-1]
来源：http://hz.bjfxy.top/gtihfyjtlq.html

PHP:  strrev($s);
来源：http://hz.birdmap.top/gtzfafonbe.html

JS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtalsqadoz.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtqbsmetql.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xinyue.icu/gtewarnvcb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.fzhhl.top/gtcbxiekpy.html

Ruby: s.reverse
来源：http://hz.daria6918.cn/gtcpwjzddj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtnowguxro.html

[E12] 统计某字符出现次数
来源：http://hz.zhiwuduotai.top/gtikmydvti.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtwvihcbgh.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gttwocuvec.html

JS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtsmsghodi.html

TS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtbzhybfmn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gttfolpbfq.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtagmhgzfu.html

Ruby: s.count("a")
来源：http://hz.tianlin.xyz/gttstjxaaq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gthlwoeonm.html

[E13] 逐字符遍历
来源：http://hz.hfpthk.cn/gttowhxhtc.html

Py:   for ch in s: print(ch)
来源：http://hz.c1oappe.top/gtpdhmpard.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hysaishi.cn/gtbiavemps.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtjkxgtmes.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gtyqifbsic.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtbomleuvj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangtech.top/gtaqydzvne.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gtqzjusfeo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtkerhsreb.html

[E14] URL 编码与 Base64
来源：http://hz.fzhhl.top/gtigqddhtt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gogol.net.cn/gtrjlhjzls.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.birdmap.top/gtszekpfvs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtmgyoguip.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgufenzy.top/gttqszipcq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtnuidozdu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xinyue.icu/gtlhiyvdkc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cqqwz.cn/gtdyxdtfgv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhongyouzk.top/gtqdwnjmod.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gtfflabldv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhaomingkeji.xyz/gtaritbtjm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daria6918.cn/gtcrecjjin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtdnmxsyct.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ppjwa.cn/gtsenedwyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtdaxwsaep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtlroemhlt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ehwqpu.com/gtlyrhpptg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxinkj.top/gtcpbbjxqd.html

[E16] 数字千分位
来源：http://hz.yvedp.cn/gteruakbmc.html

Py:   f"{1234567:,}"
来源：http://hz.c1oappe.top/gtcoxhgkel.html

PHP:  number_format(1234567);
来源：http://hz.tianlin.xyz/gtcihrplfr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gttcieunhb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtdevmyoro.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.52xcode.cn/gtkaiigxfv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtobdncnlc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtdqlslsex.html

C#:   1234567.ToString("N0")
来源：http://hz.zhoulong.xyz/gtukakchqv.html

[E17] 首字母大写
来源：http://hz.daxiang520.top/gtqdxgnspx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sxryk.cn/gtoigrjafn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shangyingyoupin.top/gtdeayhehj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtjtfweqyr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtmgdhyahz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gtywspmgqe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj202588.top/gtetvrsfoh.html

Ruby: s.capitalize
来源：http://hz.zhaomingkeji.xyz/gthxmkxvoz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daria6918.cn/gtsodehnvg.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtewqtsvgp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.bjfxy.top/gtbffhjkhg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtftublcms.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtlohresyc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.mhx1999.top/gtzwytwhwo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xziqi.cn/gtvatfafnu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gthodibsrf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gzhubu.top/gtkzalolnr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tanke756.top/gtrkdigglr.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtdnvusuai.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtaqoqpust.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.feifeiyinyue.top/gtmdlggzbe.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtkkxmwlet.html

TS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtkdokrses.html

Java: s.lines().toList()
来源：http://hz.gotoacloud.top/gtyihbsvut.html

Go:   strings.Split(s, "\n")
来源：http://hz.fengsongda.top/gtoxukphuh.html

Ruby: s.lines
来源：http://hz.ivvv.top/gtquoihtvw.html

C#:   s.Split('\n')
来源：http://hz.daria6918.cn/gtcskfvpky.html

[E20] 判断字符串是否为空
来源：http://hz.cucudq.cn/gtluylezpg.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtlnljvmed.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.9152youxi.cn/gtjqcbtmtg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hfpthk.cn/gttiqfdwyw.html

TS:   if (s === "") {}
来源：http://hz.cashguo.top/gtxvkwydzn.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtcmtaheka.html

Go:   if s == "" {}
来源：http://hz.vqdsnc.cn/gtnusrthdl.html

Ruby: if s.empty?
来源：http://hz.smart0.xyz/gtewkihnpa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shangyingyoupin.top/gttrquklom.html

[E21] 超长截断加省略号
来源：http://hz.yongpay.top/gtdrcnzgbz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xingfuxueyuan.xyz/gtkwoocktb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cqqwz.cn/gtybqylhap.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtxldzbbyc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtauajnneq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtbmneutzw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuxming.cn/gtozlpeion.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dashuyun.cn/gtzwhtrdwf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.52xcode.cn/gtimphiimx.html

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gtyeezynyx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnxiangtu.top/gtumebgftu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtttlumxea.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtqrtzhdvi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtliaipqmr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtimgyxzmb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gtuaozklvi.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtutvrgrnz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtpskscmvo.html

================================================================================
来源：http://hz.redwolf501.top/gtnthnythz.html

F. 文件与目录
来源：http://hz.ppjwa.cn/gtwymqsksy.html

================================================================================
来源：http://hz.tanke756.top/gthenuvixh.html

[F01] 读取整个文件
来源：http://hz.cashguo.top/gtoxnkfqyf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cqqwz.cn/gtenwhrouc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigufen.top/gtrieqvhnh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtbnbztmkr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtfxdleedr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtbmuvugfo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtakhekssd.html

Ruby: File.read("a.txt")
来源：http://hz.xylfe.cn/gtfjfrjucw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hysaishi.cn/gtlgribvzj.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gtyhwhcska.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtpjjkbsll.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aibaodan.cn/gtqtvmkovc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtygplncnq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtpkeeotpp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtrolqdiid.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yueranfly.top/gtmzwszdva.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sufxvd.cn/gtwkgrnlgc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258.top/gtdahiooil.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gtdsjswezf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigufen.top/gtpvmhktto.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtdaleicrm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtcvibhagd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtqjagfyvq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.haohaochexian.top/gthkdoozni.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangkeji.top/gtisahfvlu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtytlwbpgr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtlxxjqoxr.html

[F04] 追加写入文件
来源：http://hz.jinyuanbaomall.cn/gtigxfloet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtvfjnkcyk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtvfspjbki.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtlnwkiicg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtqbtudjth.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gttakhpcdt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtcgzdwkhf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258888.top/gtxwaqnzkz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hongshengwenyu.top/gtryrbqlsd.html

[F05] 判断文件或目录是否存在
来源：http://hz.aibaodan.cn/gtuzhnitzw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gaohongyu789.top/gtwgwcvubh.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtvnrezetn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtuhielxpe.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtmrthctvq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtrhnyaete.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtikgidrci.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenzaomai.com/gttwcmouii.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxinkj.top/gttkdganhg.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gtcejcpqjp.html

Py:   os.remove("a.txt")
来源：http://hz.zhongyouzk.top/gtbuikqwap.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtxbiirkuu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtqtoaqjix.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtxqgdqvsn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtxecdwdxa.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtwlmvfruu.html

Ruby: File.delete("a.txt")
来源：http://hz.daxiang520.top/gtuupauhqx.html

C#:   File.Delete("a.txt");
来源：http://hz.nwbrower.top/gttiyjwsul.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtrmggznrg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxuanxn.top/gtbjzgkupt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtfyuavlsb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtcevwxkrb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtiakjsafj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnqzz.top/gteylnwtzb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtzlfejirh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.birdmap.top/gteuexmxfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hywenlv.cn/gtowazxsbq.html

[F08] 遍历目录
来源：http://hz.zhaomingkeji.xyz/gtnahbmyfo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.vqdsnc.cn/gtlaavrvfi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gtqqbpzrpt.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtmotyqyyo.html

TS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtcpsqejme.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtuggcvdif.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtcufwmjii.html

Ruby: Dir.children("dir")
来源：http://hz.hywenlv.cn/gtejzhvndn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.kuanghao11.cn/gtqgdrzoeh.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gtmkdqlibi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuetiantiany.cn/gtswgatyxc.html

PHP:  filesize("a.txt");
来源：http://hz.cheryme.top/gtzubytjya.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtxknqlxgx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtqnbwprwo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtzsqvcbst.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.haohaochexian.top/gtpqzdmnmg.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtsonrpdra.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hysaishi.cn/gtgkodbrxj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gtapjiulyc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtgryifafz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gtzajoiziu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtabtsnxkh.html

TS:   path.extname("a.txt")
来源：http://hz.hywenlv.cn/gtzpflkjbx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gtojrksyrt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guannengcc.top/gtzvwswxei.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtnwqeykir.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cqqwz.cn/gturebmcun.html

[F11] 复制与移动文件
来源：http://hz.yuanzhike.top/gtwoibkadz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtixmfzmet.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yonumen.top/gtttbcmmrf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtsfcpthpa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtpwqexilq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tianlin.xyz/gtskyhulqc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gzhubu.top/gtlsaoflfu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gteiwrkfxc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gtszzzcfxu.html

[F12] CSV 读写
来源：http://hz.shzxlz.cn/gtzexloguz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtbqdfptwx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gtbvjzvmzu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtvhdjbpqc.html

TS:   // 同上
来源：http://hz.feifeiyinyue.top/gtdyjsorrd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtazzvbhrh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tian-w.cn/gtozdueabh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxuanxn.top/gtoxnlccoq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtrymmdxne.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtrnieonez.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtbavjyvnh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzmjcqmmj.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtekutyxaq.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gtvgmjbhpy.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtzsrltzbw.html

JS:   class User {}
来源：http://hz.zhijiandao.cn/gtykrkjqbt.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtzkjoftec.html

Java: class User {}
来源：http://hz.yueranfly.top/gtsplgjjhn.html

Go:   type User struct { Name string }
来源：http://hz.pycfn.com/gtfqwowcha.html

Ruby: class User; end
来源：http://hz.sufxvd.cn/gtlymgurzc.html

C#:   class User {}
来源：http://hz.jinqigufen.top/gtcklzmang.html

[G02] 构造函数
来源：http://hz.316326.xyz/gtiuponmiw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangshuangyany.cn/gtdpmbabrw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yonumen.top/gtcpaesiyz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtltjdrbuj.html

TS:   constructor(public name: string) {}
来源：http://hz.shangyingyoupin.top/gtgnhgdsfq.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gtvylpzrvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtovdkpprz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtlzxxkxus.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zdqjudy.top/gtkxrdkaxf.html

[G03] 实例属性
来源：http://hz.cheryme.top/gtofcnbuqa.html

Py:   self.name = "x"
来源：http://hz.chenjidiqi.icu/gtjklyjess.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtccvanjia.html

JS:   this.name = "x";
来源：http://hz.nanxuanxn.top/gtjyavrdhg.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtdywxajqf.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtpksbhirx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtymkghygu.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtfinoomhg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtojabzgza.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtiwetpaoj.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtxgudzkyj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtcamjskct.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtuyxltdyl.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtjywihghe.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtmazhzutu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.snrcjt.cn/gtjtaihjjl.html

Ruby: def greet; @name; end
来源：http://hz.yj20258.top/gtjdcjolww.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtrbjqkaqa.html

[G05] 继承
来源：http://hz.wangdashe.top/gtsdkdllor.html

Py:   class Admin(User): pass
来源：http://hz.52xcode.cn/gthnbksuls.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtxgmlqqch.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtuflgzpmz.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtnocxzwht.html


<!-- 参考信息 -->