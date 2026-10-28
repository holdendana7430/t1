代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtftzghvxc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtmwjkabjy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hywenlv.cn/gtzuygxmxh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yueranfly.top/gtkcwpypsn.html

C#:   s.Replace("a", "b")
来源：http://hz.svipenyu.cn/gtcpilywsk.html

[E07] 按分隔符拆分
来源：http://hz.zhongyouzk.top/gtyquqwzoo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.vqdsnc.cn/gtkszkzhic.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gteoqxwgit.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuanzhike.top/gtkvuavzxd.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtxaxxhzel.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhongyouzk.top/gtisovuyul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xinyue.icu/gtgqaxjnfu.html

Ruby: s.split(",");  s.split
来源：http://hz.hongshengwenyu.top/gtbwjpccub.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jlsjyb.cn/gtowbxtutf.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gtcfwesrmu.html

Py:   ",".join(items)
来源：http://hz.ywan-chungtsiang.top/gtbtnvhgye.html

PHP:  implode(",", $items);
来源：http://hz.wangshuangyany.cn/gtvetshabu.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtbkfmxqkq.html

TS:   items.join(",")
来源：http://hz.hnqzz.top/gtgknzkicw.html

Java: String.join(",", items)
来源：http://hz.jinghuilouyu.cn/gtmhgqmnwk.html

Go:   strings.Join(items, ",")
来源：http://hz.hysaishi.cn/gtkwaowpfk.html

Ruby: items.join(",")
来源：http://hz.yvedp.cn/gtjhdmvqfh.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtrllyasrz.html

[E09] 去除所有空白字符
来源：http://hz.shangyingyoupin.top/gtmfltxoly.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtupiltkkv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtemhkkqzl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtyphiotlm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtjuntwzkc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtdqnozfju.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gtgzttpfvn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuanzhike.top/gtkaddrzij.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgufenzy.top/gtsqjehuvl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.daria6918.cn/gtibkdcofk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.andypj.xyz/gtwktitzhb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigufen.top/gtlpwnveuk.html

JS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtpvhrgcih.html

TS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtsbzxapfh.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtvbcrieff.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtjfqmbllz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtmzmnxbin.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dianchejie.cn/gtgpfttmlk.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gtlkyjqjyk.html

Py:   s[::-1]
来源：http://hz.zhiwuduotai.top/gtdeznjvzl.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtjwjmnkii.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtwepvbjpo.html

TS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtuoodmgys.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.smart0.xyz/gtrvzagwtg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangkeji.top/gtfqpshrmw.html

Ruby: s.reverse
来源：http://hz.316326.xyz/gtlukuvqbq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtwhuwlglx.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtsyboatgd.html

Py:   s.count("a")
来源：http://hz.yj20258888.top/gtihzguqdq.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtisgtmqei.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtixqyajel.html

TS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtnhxenkwg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shanyushiyangtech.top/gtxivcejze.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gthamhavpu.html

Ruby: s.count("a")
来源：http://hz.yj20258.top/gtsoqncozf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenjidiqi.icu/gtwmsizmpu.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gttnnmkoow.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigufen.top/gtiacvblpv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnxiangtu.top/gtggrbgndi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtxpuciplo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gtjowkyysj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxinkj.top/gtzrykkyrj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hywenlv.cn/gterglmgzk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhijiandao.cn/gtcqvqfbgl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.iojbl.cn/gtvhdfceex.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gtskcnnmrp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinyuanbaomall.cn/gtbyjfitmb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangkeji.top/gtkvlilecc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtvwhlkpzt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtnfzkmgqk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxuanxn.top/gtgrdiblap.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.vqdsnc.cn/gtwvogfwei.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj202588.top/gtxmgkneks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtyaevaeiq.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gthnzxpwhh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtikyjgiln.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtyuzgszfa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pengpengdd.cyou/gtyygxkmgv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hammf.cn/gtmfdpzwza.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dashuyun.cn/gtobrtqels.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yueranfly.top/gtnpqqepqc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yongpay.top/gtakibmkdz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jianghu66.top/gtqzklatje.html

[E16] 数字千分位
来源：http://hz.xinyue.icu/gtgqntanva.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtbofnajla.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtlnghnpyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtxzjxzfgf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gaohongyu789.top/gtomigymod.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guannengcc.top/gtdezcmwxv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtuswsosnh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gtcbbgmxhx.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258888.top/gtcqmxibrx.html

[E17] 首字母大写
来源：http://hz.vqdsnc.cn/gttecphmin.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hammf.cn/gthimbugtz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shuidangran.top/gtjyezhbyc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtjqjiwkxa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fengsongda.top/gtjfkgiwlm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yvedp.cn/gtcqydkgeh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.quarkkingdee.top/gtebufolmy.html

Ruby: s.capitalize
来源：http://hz.ehwqpu.com/gtnypnobxl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yueranfly.top/gtqzehpykx.html

[E18] 模板占位符替换
来源：http://hz.dianchejie.cn/gtuduvysim.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangdashe.top/gtkmiejeyu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinyuanbaomall.cn/gtlfxrdneq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sxryk.cn/gtfmdpfctd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtoicqlkdc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gtcggfkubk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gtfbphscja.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ehwqpu.com/gtsivvhaob.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cdnleiting.top/gtzywjburb.html

[E19] 多行文本按行拆分
来源：http://hz.jianghu66.top/gtlkeyqffs.html

Py:   s.splitlines()
来源：http://hz.chenjidiqi.icu/gtszncgsrq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtjxjevlrd.html

JS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtzkcitnan.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtmpxdsuxz.html

Java: s.lines().toList()
来源：http://hz.redwolf501.top/gtqnvalaja.html

Go:   strings.Split(s, "\n")
来源：http://hz.aizwys.cn/gtpjbslngx.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gttkevxdjc.html

C#:   s.Split('\n')
来源：http://hz.shzxlz.cn/gtokahzwpv.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258.top/gtbapjsgwc.html

Py:   if not s:
来源：http://hz.hnxiangtu.top/gtzeztdmyz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xylfe.cn/gtqdpnoqyk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yangfankeji.com/gtustgwdss.html

TS:   if (s === "") {}
来源：http://hz.jqgufenzy.top/gtljdutcyx.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtmanjaunj.html

Go:   if s == "" {}
来源：http://hz.zdqjudy.top/gthgjznbbt.html

Ruby: if s.empty?
来源：http://hz.jinghuilouyu.cn/gtdaoarzjj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sxryk.cn/gtkeqabjun.html

[E21] 超长截断加省略号
来源：http://hz.hongshengwenyu.top/gtnmnnbarm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtygkfekxv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtzxplfszr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtjgxjtjjy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtlndksqcl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtzfxlivlf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shanyushiyangkeji.top/gtemqiumrx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtelyvgerk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yanxiufei.cn/gtnapaltpn.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtfmqmrxyp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aibaodan.cn/gtlfstioqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gttvypjglt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtokckaczg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258888.top/gtmnxhvmhs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sweek.top/gtbthvqduc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtwoospxoa.html

Ruby: s.bytesize;  s.length
来源：http://hz.dianchejie.cn/gtseeabhre.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aizwys.cn/gtjixrvjbo.html

================================================================================
来源：http://hz.guannengcc.top/gtprsrbfdq.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtgrzegxkc.html

================================================================================
来源：http://hz.sysykeji.top/gtbcagvisw.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtvhixhuif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cqqwz.cn/gtimlfhock.html

PHP:  file_get_contents("a.txt");
来源：http://hz.birdmap.top/gtgppkibbq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangtech.top/gtkvixzpqt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhixingplan.top/gtkfgaatei.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtkpylizev.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.mhx1999.top/gtdymgjfix.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtuvggcirb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtqwnxpors.html

[F02] 逐行读取文件
来源：http://hz.pengpengdd.cyou/gttbmovymj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xylfe.cn/gtttwlouqw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtxswnrxwy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtuevsytvy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtqpytenrz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtnotkcxqj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.svipenyu.cn/gtlveaifgb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.9152youxi.cn/gtyrvmgjgf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenlongwang.top/gthfivoqtm.html

[F03] 写入文件（覆盖）
来源：http://hz.52xcode.cn/gtwhrpxhaf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jlsjyb.cn/gtdlgqvinn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gthpupfvdr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtfuewlaig.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtltkomvzb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtlgbedghg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gzhubu.top/gtdwbgkocr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtphihnooc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.havefunace.top/gtfrijppbq.html

[F04] 追加写入文件
来源：http://hz.sysykeji.top/gtxssnhicj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenjidiqi.icu/gthsqzgyrb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shangyingyoupin.top/gthbsjgmgj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtdlrtirqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtqsifjkwe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtpgmijavg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gthrwmejxs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj202588.top/gtjdrwexul.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtwwehydlp.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gtidjuitwc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtgdbmjees.html

PHP:  file_exists("a.txt");
来源：http://hz.meibo888.top/gtjspakogq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtydgxerpb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtqdeyeurn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtrrcxhfep.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtteegndln.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenjidiqi.icu/gtccgyleof.html

C#:   File.Exists("a.txt")
来源：http://hz.vqdsnc.cn/gtpkcviwcz.html

[F06] 删除文件
来源：http://hz.hnqzz.top/gtukvowkwh.html

Py:   os.remove("a.txt")
来源：http://hz.tanke756.top/gtflfjpaqn.html

PHP:  unlink("a.txt");
来源：http://hz.meibo888.top/gtwfjqszph.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtlrdyulek.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtdxwxxsxt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gteusnhvzn.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtiyjkrquu.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gtmluuejnd.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtfmoygoey.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtbhaiehhn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gtjpusfepr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gtenbscral.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtglosibmx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtxjhsdcoj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtxrnucift.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cdnleiting.top/gtwhgnxniv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yueranfly.top/gtazixlzjm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gtyyptwybh.html

[F08] 遍历目录
来源：http://hz.chenlongwang.top/gttlqrrwcm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtuaoypzmq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuanzhike.top/gtlbkphsaz.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtqheqrjtl.html

TS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtpvwxwbew.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtncmlhrfv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtmchtoaai.html

Ruby: Dir.children("dir")
来源：http://hz.aibaodan.cn/gtbfqexbug.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xziqi.cn/gttnjuiczj.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gtctfbnenh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtmnhatoqk.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtaqvwkfvz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtxwcdrfth.html

TS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtjwnfudqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gteebnpddi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jianghu66.top/gtgvuxqbxo.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdvbtvifb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnqzz.top/gtjfncrmgq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtmdvvohar.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtqpoqcyhy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gthyczqwab.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtbnbdxgva.html

TS:   path.extname("a.txt")
来源：http://hz.316326.xyz/gtdyxdeixd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtsdpphsqb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gtzxgdraji.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtyfzdvfdn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.9152youxi.cn/gtdkmjefqs.html

[F11] 复制与移动文件
来源：http://hz.cqqwz.cn/gtisvoatrp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtkgievcnv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ehwqpu.com/gtcshupmmi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtjfggcinv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtqjlphydt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhijiandao.cn/gtnrxpzzqq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gttxreefra.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtxsyfwfvg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtdhobawfb.html

[F12] CSV 读写
来源：http://hz.zhijiandao.cn/gtkblqtodb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtzxmqqdns.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gttgzeiqlw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtoubzljvi.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtszobwpfc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.feifeiyinyue.top/gtrqrqvtok.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gteumchccd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtzkquvcoh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.bjfxy.top/gtalygcriv.html

================================================================================
来源：http://hz.smart0.xyz/gtadbdwiea.html

G. 面向对象
来源：http://hz.havefunace.top/gtkwrolyap.html

================================================================================
来源：http://hz.nwbrower.top/gtffaggcay.html

[G01] 定义类
来源：http://hz.yj202588.top/gtupvhcist.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtyyupfqle.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtmozbmcyg.html

JS:   class User {}
来源：http://hz.zdqjudy.top/gtzxsneaor.html

TS:   class User { name: string = ""; }
来源：http://hz.zycfv.cn/gttljizomy.html

Java: class User {}
来源：http://hz.daxiang520.top/gtzjnasqgy.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtvdhcsjxr.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtpfnrjhhi.html

C#:   class User {}
来源：http://hz.guannengcc.top/gtyqanrrxf.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtyocvtemy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgufenzy.top/gthavunior.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhijiandao.cn/gtotxqpcar.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtbratfrtl.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigufen.top/gtnitrrlbb.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtddaosqty.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fzhhl.top/gtwozakpzs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xziqi.cn/gtvisetvzs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gtzsvprgqq.html

[G03] 实例属性
来源：http://hz.shuidangran.top/gtacgzpsmo.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtduodvklk.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtfeovjalz.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtgxbqvcrg.html

TS:   name: string = "x";
来源：http://hz.yonumen.top/gtzwjocpvg.html

Java: private String name;
来源：http://hz.fzhhl.top/gtncvsrbnl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtvqwkmdam.html

Ruby: @name = "x"
来源：http://hz.tanke756.top/gtktftttgy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtlbanakgg.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtsqildjvg.html

Py:   def greet(self): return self.name
来源：http://hz.quarkkingdee.top/gtqqpzdcwz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtkzrbiwxs.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtdjmtyidw.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtjlcregfz.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gthmpmwbtc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gttprqtqsy.html

Ruby: def greet; @name; end
来源：http://hz.cucudq.cn/gttreyhgnz.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtxvmbfyfi.html

[G05] 继承
来源：http://hz.shanyushiyangkeji.top/gtfyhrvuas.html


<!-- 参考信息 -->