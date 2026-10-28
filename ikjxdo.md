代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.zhoulong.xyz/gtemwlfmbp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sweek.top/gtmmudxdqc.html

[E08] 数组按分隔符合并
来源：http://hz.haohaochexian.top/gtgqysyqkh.html

Py:   ",".join(items)
来源：http://hz.zycfv.cn/gtummecuiq.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gtvtvbkpfx.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gtishzssop.html

TS:   items.join(",")
来源：http://hz.sxryk.cn/gtdcseqmxn.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtfodowmhq.html

Go:   strings.Join(items, ",")
来源：http://hz.fzhhl.top/gtwximcbkp.html

Ruby: items.join(",")
来源：http://hz.andypj.xyz/gtvuajwuoy.html

C#:   string.Join(",", items)
来源：http://hz.0kj1m.cn/gtmcjcjbpo.html

[E09] 去除所有空白字符
来源：http://hz.316326.xyz/gtjoxlxdbc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gtdgylrqfd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtadkmawbj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtcejeiqqk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtraducltf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gtsifldfep.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangshuangyany.cn/gtbjsrhfzh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gotoacloud.top/gtkssnhdjr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xziqi.cn/gtquwsktzk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gaohongyu789.top/gtsyrtriaw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtpsqouquf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hfpthk.cn/gtsbctqrur.html

JS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtydxctdxm.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgufenzy.top/gtrqhpabih.html

Java: String.format("%03d", 7)
来源：http://hz.fzhhl.top/gtviwvnwuz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtinrwnjuo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtgvjdsuwn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.52xcode.cn/gteaoydneg.html

[E11] 反转字符串
来源：http://hz.yvedp.cn/gtttxyjnct.html

Py:   s[::-1]
来源：http://hz.jianghu66.top/gtlnkkvrmc.html

PHP:  strrev($s);
来源：http://hz.yonumen.top/gtqkgjuhrv.html

JS:   [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtstbvubud.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtqsghefhe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zycfv.cn/gtpqryvlgu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.daxiang520.top/gtwztnhqyw.html

Ruby: s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtpjbjyzuz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtqmzwgjeu.html

[E12] 统计某字符出现次数
来源：http://hz.zycfv.cn/gthdyhvktj.html

Py:   s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtcseqtktq.html

PHP:  substr_count($s, "a");
来源：http://hz.zhixingplan.top/gtjetigfze.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtgaxsmtre.html

TS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gttrlynncd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258.top/gtjsllnmfr.html

Go:   strings.Count(s, "a")
来源：http://hz.nwbrower.top/gtzfterjio.html

Ruby: s.count("a")
来源：http://hz.bjfxy.top/gtbjlxcync.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtezqvfgzn.html

[E13] 逐字符遍历
来源：http://hz.jinqigufen.top/gtibkjebid.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtkijfjnau.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtuhgmcxpm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtmjplvvyt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtberhcjqj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhiwuduotai.top/gtaxlzqjws.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fengsongda.top/gtgtcisphk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgfzy.top/gtvxxfsfbu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxuanxn.top/gthivjjgjc.html

[E14] URL 编码与 Base64
来源：http://hz.jqgfzy.top/gtjblmeixw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtzyvyqtbr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.vqdsnc.cn/gtoxpzjxzh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenlongwang.top/gtyqjkzlah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtiupkmpgo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuetiantiany.cn/gtednhnmkx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxuanxn.top/gtwpcclpyi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.bjfxy.top/gtjrnclqif.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtxxmzmorj.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtcnblacpr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sufxvd.cn/gtfxnckqvm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtkayfjxol.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtwtsiqvvt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gtkwfrvnht.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuanzx.com/gtmfvupvfb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtbhkoflxg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gtrpygowzk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gthypzwalb.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gtjvlgcmbq.html

Py:   f"{1234567:,}"
来源：http://hz.dashuyun.cn/gtixinnrdf.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtvfhjjsof.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtauxkkhxt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtfagyojwu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xziqi.cn/gtpwvhcrbb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gtfvztkehe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhengqikj.top/gtgsfsrekf.html

C#:   1234567.ToString("N0")
来源：http://hz.xziqi.cn/gtwoitazdg.html

[E17] 首字母大写
来源：http://hz.dashuyun.cn/gtecmailnd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtbeetgiul.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtpnjzswix.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtvamahhdw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtxkpvabgj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guowangkeji.top/gtmrybmpqe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gtjxdmuqcz.html

Ruby: s.capitalize
来源：http://hz.cashguo.top/gtynbkajqb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtwwreojhs.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtbxsmgbil.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gttunpmbdg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtzbqyahkl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtphpftgnb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtuzimxbml.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hywenlv.cn/gteywomyll.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jianghu66.top/gtigpjficp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxuanxn.top/gtnxcdnlse.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.mhx1999.top/gtseyetaen.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gteuvcgabg.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtfvpndsmy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtefaduktp.html

JS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtrsyilfde.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtvspwqepi.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gtvemxjwmd.html

Go:   strings.Split(s, "\n")
来源：http://hz.yvedp.cn/gttguqpxpe.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtxikzadml.html

C#:   s.Split('\n')
来源：http://hz.zhongyouzk.top/gttbwjjzif.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigufen.top/gtzvdsdidk.html

Py:   if not s:
来源：http://hz.jinyuanbaomall.cn/gtleddyamb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yongpay.top/gtsqigphct.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.mhx1999.top/gtpudziskg.html

TS:   if (s === "") {}
来源：http://hz.haohaochexian.top/gtpiweyacc.html

Java: if (s.isEmpty()) {}
来源：http://hz.tian-w.cn/gtvmooudmy.html

Go:   if s == "" {}
来源：http://hz.nanxuanxn.top/gtokgfqwur.html

Ruby: if s.empty?
来源：http://hz.yvedp.cn/gtnaurrygj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtanxaslza.html

[E21] 超长截断加省略号
来源：http://hz.gaohongyu789.top/gtaokrslhx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgufenzy.top/gtbeyuwaix.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtxywqrstu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtyvrepufk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtufotgsrq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gthkgrmmby.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ywan-chungtsiang.top/gtusryehpd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtjjppkiit.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gtlhifxepz.html

[E22] 字节长度与字符长度
来源：http://hz.yongpay.top/gtzqmgwkhs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gtetynxapr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtpydxbsnb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtfwfgbazl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtcbkkhunj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.vqdsnc.cn/gtygxmqate.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gaohongyu789.top/gtnjcfokjt.html

Ruby: s.bytesize;  s.length
来源：http://hz.vqdsnc.cn/gtinatzwgh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gtkaxlfnwg.html

================================================================================
来源：http://hz.jianghu66.top/gtqdubofnq.html

F. 文件与目录
来源：http://hz.ppjwa.cn/gtqnbpmato.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkjajtmoi.html

[F01] 读取整个文件
来源：http://hz.daria6918.cn/gtwcuxzyqo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnqzz.top/gtedzaiuhy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtludpfclm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yanxiufei.cn/gtcysdmknt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuanzx.com/gthmsgaxrk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtaaobnbxn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuxming.cn/gteexawjkf.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtwibbsxxq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hywenlv.cn/gtxszafjna.html

[F02] 逐行读取文件
来源：http://hz.quarkkingdee.top/gtjnbzxhwp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shzxlz.cn/gtuyyazcdv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtnqzhckvi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtdnuccpvq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtcophlfhj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtqrectfmm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtpeuiivmm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangshuangyany.cn/gtiyysfbzb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.quarkkingdee.top/gtbkgtgqfh.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtoxscfdii.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.316326.xyz/gtiwlxcqll.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtlfucmahm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtmpdvabrz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtintzfcpi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtdggpdifu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xuetiantiany.cn/gthgilsmid.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuxming.cn/gtuvhlmjuz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cashguo.top/gtjwriuxpx.html

[F04] 追加写入文件
来源：http://hz.yongpay.top/gtwnrmtift.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hywenlv.cn/gtbjnikqpj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.vqdsnc.cn/gtehzbayfh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtcdzpyjvt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtnapvykvq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.9152youxi.cn/gtevvmmqyi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtfsmuywvl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gtscetfqpo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangdashe.top/gtgyvfstfg.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtmbdqkttw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aizwys.cn/gtlstfcjmn.html

PHP:  file_exists("a.txt");
来源：http://hz.gotoacloud.top/gtdyvepeni.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtmcncyysq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtvsnwlwvo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtgexokmgv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yongpay.top/gtbyrhwmia.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangtech.top/gttnvpmfoo.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtnhkodhkx.html

[F06] 删除文件
来源：http://hz.ywan-chungtsiang.top/gtkdtxmysm.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gtyixmwdzc.html

PHP:  unlink("a.txt");
来源：http://hz.316326.xyz/gtoecsykmn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtxkqnmcbz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtkrjyeoku.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gthhlyipks.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtaokwsvqz.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gthymfloli.html

C#:   File.Delete("a.txt");
来源：http://hz.jiagoushi.top/gtocxjfthl.html

[F07] 创建目录（含多级）
来源：http://hz.yj202588.top/gtmkwrernc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtjpknicqo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jiagoushi.top/gtdcfukshs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtxxfojlhj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtaaqwkjvd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinyuanbaomall.cn/gtgzwplsvk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sxryk.cn/gtyijrqogb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hammf.cn/gtovqejgyr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtydzqjmnn.html

[F08] 遍历目录
来源：http://hz.snrcjt.cn/gtjsnemirl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fzhhl.top/gtcijmytax.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.svipenyu.cn/gtaredmidy.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtdmgkzegz.html

TS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtumtxdfox.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtutsjuent.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgfzy.top/gthnjhalck.html

Ruby: Dir.children("dir")
来源：http://hz.zycfv.cn/gtknqamibw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtaoccmxuq.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gtzmysbfmy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gtskwwdwgx.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtfljlkvim.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gtmfejymfe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtwbkbuszv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtzlcymwrc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gttvhrrzkb.html

Ruby: File.size("a.txt")
来源：http://hz.zhengqikj.top/gtnivepulu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gogol.net.cn/gtmocvmocp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hammf.cn/gtatqnmflq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtlgzrvkko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gaohongyu789.top/gtinkwpbph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtsokeesxg.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gtkomtktks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.mhx1999.top/gtzponafzm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gzhubu.top/gtwjszekda.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gttoiciyto.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtyhnbskez.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gtazajsahr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtlcymnokx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtfcfxaghn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtitznmaie.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtqrhxnikk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gtaxlwbtqh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydzc1.top/gtkrfhghye.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtwsbsfhjq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gtknjatrow.html

[F12] CSV 读写
来源：http://hz.sweek.top/gtgehjjpih.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gotoacloud.top/gtgmjwgpoi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxinkj.top/gteasynhpa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gtusunlqlo.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtduyqmihj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtxmjjcxjl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtvcqvatwy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.kuanghao11.cn/gtfadkdrdc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sysykeji.top/gtlvlbyoyj.html

================================================================================
来源：http://hz.jyoumei.cn/gtomqjxwmw.html

G. 面向对象
来源：http://hz.smart0.xyz/gtanvbyxou.html

================================================================================
来源：http://hz.vqdsnc.cn/gtfaoenpnc.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtiqiwddma.html

Py:   class User: pass
来源：http://hz.0kj1m.cn/gtvunqrply.html

PHP:  class User {}
来源：http://hz.daxiang520.top/gtydazvldt.html

JS:   class User {}
来源：http://hz.daria6918.cn/gttdaxcrft.html

TS:   class User { name: string = ""; }
来源：http://hz.sxryk.cn/gtbgmfzyuk.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtnxkubiwx.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtaexnqadm.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gtbojrrler.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtwbpohjxp.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtpgzgnvyf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtugzmndnv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sufxvd.cn/gtnfqboyvk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydzc1.top/gtstqdtsbp.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtdgfjifux.html

Java: User(String name) { this.name = name; }
来源：http://hz.sxryk.cn/gtjwyjxkvk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtcsnhcqid.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhongyouzk.top/gttwhqkcqq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtwchkjmii.html

[G03] 实例属性
来源：http://hz.hnxiangtu.top/gtltngzlml.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtnyrdmeon.html

PHP:  public string $name = "x";
来源：http://hz.gogol.net.cn/gtseciyshl.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtgmqfhoan.html

TS:   name: string = "x";
来源：http://hz.sxryk.cn/gtrngumqqj.html

Java: private String name;
来源：http://hz.pengpengdd.cyou/gtkrnvupgd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ivvv.top/gtkeluxnsm.html

Ruby: @name = "x"
来源：http://hz.svipenyu.cn/gtsiszrerx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yvedp.cn/gtorqrzerz.html

[G04] 定义方法
来源：http://hz.meibo888.top/gtamsippyr.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gtgeaghzch.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtdrdtejem.html

JS:   greet() { return this.name; }
来源：http://hz.chenlongwang.top/gtkmewojoy.html

TS:   greet(): string { return this.name; }
来源：http://hz.jianghu66.top/gtvuavizyh.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gtrxjhdvwc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aibaodan.cn/gtvzwssbxq.html

Ruby: def greet; @name; end
来源：http://hz.gzhubu.top/gtwtxmuooh.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtatxcylce.html

[G05] 继承
来源：http://hz.cdnleiting.top/gticgnihwg.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtkqzfujlr.html

PHP:  class Admin extends User {}
来源：http://hz.nanxinkj.top/gtrqwzmgtn.html

JS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtvhtahvzx.html

TS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gthqtryobn.html

Java: class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtnscpiyyv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtboskvrtb.html

Ruby: class Admin < User; end
来源：http://hz.dianchejie.cn/gtjgbiedvj.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtdefalboz.html

[G06] 重写方法
来源：http://hz.kuanghao11.cn/gtgceqktty.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtkpomrzjw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtlwitftsz.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gthipjrqwy.html


<!-- 参考信息 -->