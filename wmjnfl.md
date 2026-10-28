代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtionxbfix.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtyohhycot.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daxiang520.top/gtafzhqhni.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yonumen.top/gtibjbzwxe.html

C#:   s.Replace("a", "b")
来源：http://hz.9152youxi.cn/gtrdqbxwmg.html

[E07] 按分隔符拆分
来源：http://hz.yj20258888.top/gthdrpybug.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhongyouzk.top/gtlxkbytjf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cqqwz.cn/gtqivnpllr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zdqjudy.top/gtugytlvdr.html

TS:   s.split(",")
来源：http://hz.yj20258888.top/gtclohouae.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuanzx.com/gtwtablziw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cucudq.cn/gtesxgwvbb.html

Ruby: s.split(",");  s.split
来源：http://hz.snrcjt.cn/gtngnneeie.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhengqikj.top/gtwtcazspo.html

[E08] 数组按分隔符合并
来源：http://hz.ybcxt.top/gtibtiirpc.html

Py:   ",".join(items)
来源：http://hz.fzhhl.top/gtezilxega.html

PHP:  implode(",", $items);
来源：http://hz.yanxiufei.cn/gtbrgqbpxe.html

JS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtcqslstvg.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtquzduyua.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtiinrfknw.html

Go:   strings.Join(items, ",")
来源：http://hz.yvedp.cn/gthnsgzoqd.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtgjtttxgi.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gtrjeamkcq.html

[E09] 去除所有空白字符
来源：http://hz.pycfn.com/gttfmshxfj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.meibo888.top/gtcowxprgv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gteybfbycn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtijubfbuk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtwuczmvsp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtevhiyclz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cdnleiting.top/gthuyaqfew.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sweek.top/gtjzyziotx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtehwsjyqt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xingfuxueyuan.xyz/gthafzujkp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daria6918.cn/gtqkrjqqyd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hysaishi.cn/gtkwvrakqs.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtsifbjazm.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtztcdkgku.html

Java: String.format("%03d", 7)
来源：http://hz.jyoumei.cn/gtderzedeu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xziqi.cn/gtwwhfltid.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guannengcc.top/gtaxaebcuh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtgvyhxudc.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtlxkimmdi.html

Py:   s[::-1]
来源：http://hz.aibaodan.cn/gtjpewclbv.html

PHP:  strrev($s);
来源：http://hz.dianchejie.cn/gtffzhenhj.html

JS:   [...s].reverse().join("")
来源：http://hz.ivvv.top/gtayegzlcu.html

TS:   [...s].reverse().join("")
来源：http://hz.ivvv.top/gtusqyajev.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxuanxn.top/gtqcunnvrg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtqdhivmmm.html

Ruby: s.reverse
来源：http://hz.pengpengdd.cyou/gtoihfzfny.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtbkybvsmk.html

[E12] 统计某字符出现次数
来源：http://hz.havefunace.top/gtokyzuoeb.html

Py:   s.count("a")
来源：http://hz.gogol.net.cn/gtrjtzdbdr.html

PHP:  substr_count($s, "a");
来源：http://hz.yanxiufei.cn/gtnqbjufcb.html

JS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtzxnvsqcx.html

TS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gthmbfgwpq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtwffalpaj.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtxnwqeout.html

Ruby: s.count("a")
来源：http://hz.xinyue.icu/gtfqojfprx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zycfv.cn/gtzrctcokn.html

[E13] 逐字符遍历
来源：http://hz.zdqjudy.top/gtdgeeoodx.html

Py:   for ch in s: print(ch)
来源：http://hz.0kj1m.cn/gtovfwrtqh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtgcvtyeix.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtnxulcfyq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtsxgpgtjj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangdashe.top/gtdibcxvpg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtwanxtyls.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.bjfxy.top/gtwurvhwcq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shuidangran.top/gtvwylfspg.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gtmlgtbftc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangtech.top/gthvngabte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gtdenrwdsi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinyuanbaomall.cn/gtthyomonp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gttgkogexq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtrznilyqt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtakbtlgnp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.52xcode.cn/gtuycsmbnh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtasmsyabm.html

[E15] HTML 转义 / 反转义
来源：http://hz.316326.xyz/gtxjvxwmvr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtzgdqalxz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtpmhuopqp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenjidiqi.icu/gtlnwymkyn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhijiandao.cn/gtwlqjvorp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gttozbjvhd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cdnleiting.top/gtiugooyac.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtjqztwhbv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtstrotqfl.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gtchoyihpb.html

Py:   f"{1234567:,}"
来源：http://hz.zhiwuduotai.top/gtzqdjtbaj.html

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtksiuapum.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtcoahoaep.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtfvtmavjw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnxiangtu.top/gtkuawcgyn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtjhlvxiug.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtqgaeyqnu.html

C#:   1234567.ToString("N0")
来源：http://hz.zhongyouzk.top/gtkhclxgpx.html

[E17] 首字母大写
来源：http://hz.haohaochexian.top/gthsqzqoty.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtjgoaqfmv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtyrrliylf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtejroquzv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtkngrfvju.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigufen.top/gtnpzukvez.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinyuanbaomall.cn/gtyvgxrsus.html

Ruby: s.capitalize
来源：http://hz.guannengcc.top/gtxnangore.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cqqwz.cn/gtkzslhrak.html

[E18] 模板占位符替换
来源：http://hz.zhixingplan.top/gtkbxbxcoi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gtvwjcnlaj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gtatpayviz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtfyzypfrk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtaolocgwu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shzxlz.cn/gtxgckgwfq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.quarkkingdee.top/gtpcwmczeh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtmxhvpqjt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gtpqlhiajl.html

[E19] 多行文本按行拆分
来源：http://hz.jinyuanbaomall.cn/gtarlkojjz.html

Py:   s.splitlines()
来源：http://hz.yongpay.top/gtxhfwgdxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gturomethb.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtbpilyono.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtqgkcpacf.html

Java: s.lines().toList()
来源：http://hz.aibaodan.cn/gtnhvprlky.html

Go:   strings.Split(s, "\n")
来源：http://hz.fengsongda.top/gtduehbjhd.html

Ruby: s.lines
来源：http://hz.jlsjyb.cn/gtxlqjyzyv.html

C#:   s.Split('\n')
来源：http://hz.yj20258888.top/gtknwqxzdi.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtrabrjdki.html

Py:   if not s:
来源：http://hz.sweek.top/gtsldwmmvt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jianghu66.top/gtltcbzujg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtoizktqje.html

TS:   if (s === "") {}
来源：http://hz.snrcjt.cn/gtxfkgfrcc.html

Java: if (s.isEmpty()) {}
来源：http://hz.hammf.cn/gtyqcddlxv.html

Go:   if s == "" {}
来源：http://hz.yj20258888.top/gtphnuwwox.html

Ruby: if s.empty?
来源：http://hz.yangfankeji.com/gtvdclsggy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtrypbqgre.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtjgtfsglx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtlfgfougv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cucudq.cn/gtghfiimul.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtvlnfgxml.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtofholwdx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtseafxyel.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gtxsotrggs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dianchejie.cn/gtudrvhucp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cheryme.top/gtlnoxksfd.html

[E22] 字节长度与字符长度
来源：http://hz.chenlongwang.top/gttnzsdssi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.snrcjt.cn/gteksovgyw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtuthnkmlr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtqojuqfia.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtrapuhdfr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gtyahcjzcz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gtwzudmkfx.html

Ruby: s.bytesize;  s.length
来源：http://hz.gaohongyu789.top/gtbjyzjwoy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gtpjgvpzgx.html

================================================================================
来源：http://hz.shzxlz.cn/gthfkbmafy.html

F. 文件与目录
来源：http://hz.yongpay.top/gtpgjivbzl.html

================================================================================
来源：http://hz.jqgufenzy.top/gtuaotnhsa.html

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtznczebmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtqlfqkjyc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtzqetzyqd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.quarkkingdee.top/gtopmxpqie.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gzhubu.top/gtndgrfohn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtmihsefpk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtvaouijmj.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtdobftwoa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sxryk.cn/gtwyycjjlt.html

[F02] 逐行读取文件
来源：http://hz.hnqzz.top/gtryhojjhs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.feifeiyinyue.top/gtbxgcdiwb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gtyjeeopzb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtzpgrwtcx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtxyrlkurg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtzrzyjsuj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtttmmtpnv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gteglbcdgp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtpfshiels.html

[F03] 写入文件（覆盖）
来源：http://hz.quarkkingdee.top/gtfzfubtym.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dashuyun.cn/gtydavybia.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtobrpihbv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtjwvpxesv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtotjtwlza.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.svipenyu.cn/gtnriorznl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yuxming.cn/gtjtldgcal.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigufen.top/gtnziukldi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtuycdrnmn.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gtxddklxyn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daria6918.cn/gtrposknpn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yanxiufei.cn/gtpdhaayso.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtuwifujou.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtvkdrczdm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtctyvmkcf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yongpay.top/gtyljexfsu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.redwolf501.top/gttwmyxaol.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangdashe.top/gtkgsnkhgz.html

[F05] 判断文件或目录是否存在
来源：http://hz.jlsjyb.cn/gtgjybsnpu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtduxdgokr.html

PHP:  file_exists("a.txt");
来源：http://hz.316326.xyz/gtiocrsumy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtmacxcpqp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtandhagws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtkkpeocmd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cucudq.cn/gtklppqwxw.html

Ruby: File.exist?("a.txt")
来源：http://hz.cheryme.top/gtzdepbrta.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtpjwtembt.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtmjoiquwv.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gtkhhlonkf.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtdvxzslxm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtyzbvdwvk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtmtxvgkqz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtevyozhcl.html

Go:   os.Remove("a.txt")
来源：http://hz.yuxming.cn/gtbbsoyoky.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtqzgswrwm.html

C#:   File.Delete("a.txt");
来源：http://hz.chenlongwang.top/gtenzofioc.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gtpdklegfb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258.top/gtdepokwpy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gtrymdmydp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gttkxxykyu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtloebnjbh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtveqbxtum.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cdnleiting.top/gtzchkcffe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ywan-chungtsiang.top/gttcbhawlz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daria6918.cn/gtkhrxqlvx.html

[F08] 遍历目录
来源：http://hz.jinghuilouyu.cn/gtqnetduyj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtlnzohpov.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtqrbvwhmm.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtqycckpyk.html

TS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtljcncqsc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtuzmcitcv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gtgjypgler.html

Ruby: Dir.children("dir")
来源：http://hz.xuanzx.com/gtwkdhvaki.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtxfgmkiox.html

[F09] 获取文件大小
来源：http://hz.tianlin.xyz/gtdztkaoqo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.0kj1m.cn/gtziqvkpuf.html

PHP:  filesize("a.txt");
来源：http://hz.snrcjt.cn/gtsacqpryp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtcbyjyitt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtbqjavfvl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtmggnjlqn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtthvvehjb.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtucqefkdn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xziqi.cn/gtuyvsvddq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtmsaqqtmu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtovnkbxxg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenjidiqi.icu/gtmmhejyta.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtytayikqz.html

TS:   path.extname("a.txt")
来源：http://hz.fengsongda.top/gtavqjilit.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuanzx.com/gtdillcnad.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258888.top/gtmjsqvlcl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtaooplaax.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtxtqeineu.html

[F11] 复制与移动文件
来源：http://hz.hysaishi.cn/gtviaspqze.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtqxvokgrn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258888.top/gteffgqgwy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtgtzxmidv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtczrysgzb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtvtuavhak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtxyxqnyvx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtzhplnpaa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.52xcode.cn/gtldkxgadf.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gtqlysvrrk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sufxvd.cn/gtbsobykak.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dianchejie.cn/gtszjmfgcp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtetaeklks.html

TS:   // 同上
来源：http://hz.tanke756.top/gtumqhjqjz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtlyrozdkn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gthqzjbvdg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtwnxxtuzz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shzxlz.cn/gtdkhkvcwt.html

================================================================================
来源：http://hz.ppjwa.cn/gtqoxrated.html

G. 面向对象
来源：http://hz.nanxinkj.top/gtgwkwzqfm.html

================================================================================
来源：http://hz.xuanzx.com/gtshsbuesx.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtiydzfbrw.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gtyzgwwurr.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtdrqdsdll.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gtlitgkulw.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gtwcutipde.html

Java: class User {}
来源：http://hz.ywan-chungtsiang.top/gthrizoqiz.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gtpjpsxejo.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtvoeaeenj.html

C#:   class User {}
来源：http://hz.yj20258888.top/gtybkowvns.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtnmlvedtq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtvbbajutx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangtech.top/gtchercqmn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtpjawrxro.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gthulzzoxr.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtkgqtmqfz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ivvv.top/gtszrdptck.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258.top/gtmijyuczw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yvedp.cn/gtbhnxcbea.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtrqimdwmz.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtbrjlnqgv.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtanamrlpe.html

JS:   this.name = "x";
来源：http://hz.nanxinkj.top/gtoddpxwrw.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtyoukgwgj.html

Java: private String name;
来源：http://hz.xziqi.cn/gtawsphxqw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nwbrower.top/gtdrqzjrrq.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtnobsmmjg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gttqvtlhvn.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gtpgugvana.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gtwnlgozvi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtrfazqdtl.html

JS:   greet() { return this.name; }
来源：http://hz.yvedp.cn/gtagdrdrwc.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtnldphmbj.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtwmjzqopz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtkvmdmrbq.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtjpgfpbjr.html

C#:   public string Greet() => Name;
来源：http://hz.shuidangran.top/gtywhidbxz.html

[G05] 继承
来源：http://hz.jqgfzy.top/gtcnkbpffu.html


<!-- 参考信息 -->