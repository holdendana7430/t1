代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gzhubu.top/gtcaahfkxy.html

TS:   s.split(",")
来源：http://hz.dianchejie.cn/gtcilogogi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hammf.cn/gtmrshcyyk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtgatczrti.html

Ruby: s.split(",");  s.split
来源：http://hz.aibaodan.cn/gtyobkknir.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuxming.cn/gtlehomiim.html

[E08] 数组按分隔符合并
来源：http://hz.andypj.xyz/gtktlrlqcn.html

Py:   ",".join(items)
来源：http://hz.redwolf501.top/gtgwiqtesc.html

PHP:  implode(",", $items);
来源：http://hz.jlsjyb.cn/gtmotibvxy.html

JS:   items.join(",")
来源：http://hz.cheryme.top/gtpbtrzyyf.html

TS:   items.join(",")
来源：http://hz.ivvv.top/gtfhbiisow.html

Java: String.join(",", items)
来源：http://hz.sufxvd.cn/gttfrrlwlz.html

Go:   strings.Join(items, ",")
来源：http://hz.cheryme.top/gtmizlphoc.html

Ruby: items.join(",")
来源：http://hz.ywan-chungtsiang.top/gttevfojsk.html

C#:   string.Join(",", items)
来源：http://hz.fengsongda.top/gtisxvyuif.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtghctobcn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cucudq.cn/gtkwckhwvn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenlongwang.top/gtbyursble.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtsvlbubjd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtjezzpgqy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtxooupkeg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtpakhjnjp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sxryk.cn/gtkanbewai.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gtjspddxmt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtomzemriy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.c1oappe.top/gtuytwcmuh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xingfuxueyuan.xyz/gtscgxzuhj.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtpvaggicr.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtoumrzwmz.html

Java: String.format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtlojpryrk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.haohaochexian.top/gtdvrkyeoc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtamajncpz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtcqezaipf.html

[E11] 反转字符串
来源：http://hz.fengsongda.top/gtlpxkbkev.html

Py:   s[::-1]
来源：http://hz.chenjidiqi.icu/gtontldacc.html

PHP:  strrev($s);
来源：http://hz.316326.xyz/gtlhvnwcjp.html

JS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtrthsoghi.html

TS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtrdinoqvy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuetiantiany.cn/gtxplygfiq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtwirjwnls.html

Ruby: s.reverse
来源：http://hz.hywenlv.cn/gtxfixuwmi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtjqdajmtn.html

[E12] 统计某字符出现次数
来源：http://hz.vqdsnc.cn/gtyzxtylzu.html

Py:   s.count("a")
来源：http://hz.yvedp.cn/gtanhzuxci.html

PHP:  substr_count($s, "a");
来源：http://hz.dashuyun.cn/gtiepmxdeg.html

JS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtcdxexuhn.html

TS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtixkmxvhq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtjmneuhma.html

Go:   strings.Count(s, "a")
来源：http://hz.guannengcc.top/gtrxkenxiq.html

Ruby: s.count("a")
来源：http://hz.316326.xyz/gtqwglecex.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daxiang520.top/gtczgimura.html

[E13] 逐字符遍历
来源：http://hz.ppjwa.cn/gtqgyznakw.html

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gtvppwquxg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cashguo.top/gtcgpchrax.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtvgyxdobg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gteojmeess.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jianghu66.top/gtphmutram.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cucudq.cn/gtvavcehfy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhengqikj.top/gtlzqqxojx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuetiantiany.cn/gtkfxfgzmr.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtgxbhlryw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtuguwimkf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gtxuvtysex.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gthpcdmoeb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhixingplan.top/gtdfcaqghn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ehwqpu.com/gtlsdrgnjj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gttfejgbgq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gotoacloud.top/gtqactivxt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj202588.top/gtivosmpat.html

[E15] HTML 转义 / 反转义
来源：http://hz.cucudq.cn/gtmukjzfcx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.birdmap.top/gtheabukmc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuetiantiany.cn/gtvgwyjcoc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gtcslyodja.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sysykeji.top/gthbljrrxu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xziqi.cn/gtogwouewg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhiwuduotai.top/gtidjtqhna.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.meibo888.top/gtdsikzfgn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tanke756.top/gtqdgxldgx.html

[E16] 数字千分位
来源：http://hz.ywan-chungtsiang.top/gtjywtdson.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtkwuyjdru.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtzwsabyes.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtxdwmwnsb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtkvypoqaq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hfpthk.cn/gtybhehhjc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhixingplan.top/gtcalsupvr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtyghxhqhd.html

C#:   1234567.ToString("N0")
来源：http://hz.tian-w.cn/gtyupgzcjs.html

[E17] 首字母大写
来源：http://hz.xuanzx.com/gtvtkfptie.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ppjwa.cn/gtybwjrpvs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigfzy.top/gtiulyhcxt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtpvmwgajo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtqugqgcny.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.iojbl.cn/gtaomitzsx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xziqi.cn/gthvngutjx.html

Ruby: s.capitalize
来源：http://hz.jinqigufen.top/gtbgcovrvx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aizwys.cn/gtvvbqopxl.html

[E18] 模板占位符替换
来源：http://hz.hfpthk.cn/gtcaydfsvu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtaielxaff.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gtknzuvbkb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gtpfckihxj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gthehfaoti.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tianlin.xyz/gtuywkpzji.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.kuanghao11.cn/gtpsdygywh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sweek.top/gtbvfxylra.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtjqllvlhy.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtjxmirnjb.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gtohujgwru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtjeueqpux.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtrhkljxbg.html

TS:   s.split(/\r?\n/)
来源：http://hz.daria6918.cn/gtuwtnwwqh.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtenzdlive.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gturbjqfag.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtemrbkomi.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gttackmxun.html

[E20] 判断字符串是否为空
来源：http://hz.cucudq.cn/gtsixuktul.html

Py:   if not s:
来源：http://hz.jinqigfzy.top/gtfvjsutvp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shangyingyoupin.top/gtunvpiksx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daxiang520.top/gtgwbesknl.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtctdowdca.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtuisxaufj.html

Go:   if s == "" {}
来源：http://hz.52xcode.cn/gtmpwqcocu.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangkeji.top/gtewwffptx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtbcdiyjck.html

[E21] 超长截断加省略号
来源：http://hz.guowangkeji.top/gtbftdvqbx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhengqikj.top/gthcmdtrrp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gtfseagljh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtxsvdzwnj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtlvlogjta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtrtcosxpr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guannengcc.top/gtnweovqcv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gotoacloud.top/gtzcghgdvl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtxswojvin.html

[E22] 字节长度与字符长度
来源：http://hz.xuanzx.com/gtrjfobxki.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtaeefaubm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtfsptghbj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtepccmguh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtpzbtryzt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fzhhl.top/gttfaggwyb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtdfkupcjt.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhongyouzk.top/gtgrkfqmtq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hysaishi.cn/gtpmkdkfsi.html

================================================================================
来源：http://hz.ppjwa.cn/gtqahzltad.html

F. 文件与目录
来源：http://hz.birdmap.top/gtqkxuowaw.html

================================================================================
来源：http://hz.zhoulong.xyz/gthuoambrv.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gtlzccrtfc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtggfywqbg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtvohewdql.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtdxinohdk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtmvhemdwg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtvgmwzcop.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtvexhuqxr.html

Ruby: File.read("a.txt")
来源：http://hz.jqgufenzy.top/gthhooarnf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtytdzawcq.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtuqwzdxou.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtmowrlmxk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.bjfxy.top/gtalxwezqu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtqjiugrzg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtmmtubkqd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtxkxiotni.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gaohongyu789.top/gtedvmqdye.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.feifeiyinyue.top/gtirnfdjlr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yanxiufei.cn/gtqetjpgon.html

[F03] 写入文件（覆盖）
来源：http://hz.sxryk.cn/gtfbauudxp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cqqwz.cn/gtwxogzhtp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtufbvevpj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtdnwnmsez.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtxivdaemw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.svipenyu.cn/gttgpgggrk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtkyxrhvun.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenzaomai.com/gtpfupjyvk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtescwkpts.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gthdpmkhzs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gtjjxbbcwy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cheryme.top/gtpgzfvnyx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtoosywdfj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangshuangyany.cn/gtkbrvayfp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinghuilouyu.cn/gtojosmfje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.birdmap.top/gtrbdvyhfb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuetiantiany.cn/gtpyuxhmcg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.kuanghao11.cn/gtdpwlyeuu.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtyhxeahpf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nwbrower.top/gtyhdwkahl.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtbjyatfoj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtvumpmhmj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gteutqswnc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtulkwmfvs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtywaudwlv.html

Ruby: File.exist?("a.txt")
来源：http://hz.yangfankeji.com/gtcckbgefe.html

C#:   File.Exists("a.txt")
来源：http://hz.9152youxi.cn/gthsrgpozk.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gtyhwlgiaw.html

Py:   os.remove("a.txt")
来源：http://hz.hnqzz.top/gtdilbqonx.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtdtkbrlus.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gttbveinnl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtocucnsaf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtnyfxystm.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtdrjophpc.html

Ruby: File.delete("a.txt")
来源：http://hz.316326.xyz/gtvcinzmdy.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtcxbmnzaw.html

[F07] 创建目录（含多级）
来源：http://hz.zhixingplan.top/gtjmotyhsx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtfnavpfek.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gthmzsebgk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtbmzphxqz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtovakpaow.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtfaiorrti.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shuidangran.top/gtyqejjwrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cashguo.top/gtbcxlisdr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.redwolf501.top/gtzmzaeyiy.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gtqjhdljgr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtwffwwtyf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ivvv.top/gtjqhzoxhn.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtxewnzhic.html

TS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtgbokfccj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtbicemyrv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gtnffygggt.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtbfhfgazc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtibptpqeq.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtkhbtnkhq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenjidiqi.icu/gtuqsmdtxh.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gthmpngexf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtzxontlic.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtcgvdfowq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtmtdtqqyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtstloqaps.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gtpxogknoz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtaivgefdf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aibaodan.cn/gtommphxvn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gttersflvd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj202588.top/gtmcyufkga.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtgwkqmklw.html

TS:   path.extname("a.txt")
来源：http://hz.bjfxy.top/gtphemhsaj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gthckwgquq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtcexnyert.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtjrgpwaag.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtalphbojp.html

[F11] 复制与移动文件
来源：http://hz.jiagoushi.top/gtsfmwlcui.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtcuocpibf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtfrszoelb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtmajtzscj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtustgtvym.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtgqlpzqav.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigfzy.top/gtjfdumrlq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gteeupwnsc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gtzoplckov.html

[F12] CSV 读写
来源：http://hz.daxiang520.top/gtkmqveuqq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtcjcbudhn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shangyingyoupin.top/gtagjguuni.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shzxlz.cn/gtjuoswbze.html

TS:   // 同上
来源：http://hz.gaohongyu789.top/gtivofmnab.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gtihupbbnx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fengsongda.top/gtyncsifjs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gtaneikwie.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sweek.top/gtecrkuoji.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtoqoybfir.html

G. 面向对象
来源：http://hz.havefunace.top/gtpsmrjquj.html

================================================================================
来源：http://hz.havefunace.top/gtzlvvtkko.html

[G01] 定义类
来源：http://hz.nanxuanxn.top/gtteipqhfz.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtosbmbsrl.html

PHP:  class User {}
来源：http://hz.zhijiandao.cn/gtycybflry.html

JS:   class User {}
来源：http://hz.aizwys.cn/gtenalhxes.html

TS:   class User { name: string = ""; }
来源：http://hz.yonumen.top/gtggwnjihr.html

Java: class User {}
来源：http://hz.aibaodan.cn/gtzwiabmzn.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtiibfocxm.html

Ruby: class User; end
来源：http://hz.kuanghao11.cn/gtuplabneo.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtzuthseyl.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtmrihwgsk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daxiang520.top/gtyfaulloe.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.52xcode.cn/gtwkxjaenh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtysuuydxx.html

TS:   constructor(public name: string) {}
来源：http://hz.yongpay.top/gtyefjgcqh.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtlzzdguet.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtxuyvupve.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtweyckvso.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinyuanbaomall.cn/gtxvuxmcai.html

[G03] 实例属性
来源：http://hz.hysaishi.cn/gtrofqawhv.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gttrstgqkn.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtbhcgbnrl.html

JS:   this.name = "x";
来源：http://hz.sweek.top/gteelfztnb.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gtikfongst.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtqlypnctk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gticrzvdkk.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtnvuzmtqw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtnfcauxfm.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtgepsejhx.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtaumzqnxg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sweek.top/gtlwsuztxg.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtaoulpclc.html

TS:   greet(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtypdpbedh.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtdhufdngx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuxming.cn/gttrrpcfmx.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gtmurdfhsp.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtyctqlvol.html

[G05] 继承
来源：http://hz.mhx1999.top/gtqusmckil.html

Py:   class Admin(User): pass
来源：http://hz.feifeiyinyue.top/gtpmqokjgw.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtjahomvga.html

JS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtrrmprxax.html

TS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtqfpbgeiy.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtjyclrosa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtrypgcrip.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtfdboyvmt.html

C#:   class Admin : User {}
来源：http://hz.xingfuxueyuan.xyz/gtwbnlbqns.html


<!-- 参考信息 -->