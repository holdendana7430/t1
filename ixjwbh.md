代发 wailian999

[E06] 替换子串
来源：http://hz.mhx1999.top/gtzisyvegk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yanxiufei.cn/gtxqpcearf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtpxswwwru.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtwocvbbtt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtqsphljrw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtcsjsiqef.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.andypj.xyz/gttbqyknlk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sysykeji.top/gtyvlawoey.html

C#:   s.Replace("a", "b")
来源：http://hz.ehwqpu.com/gtgxarccbi.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtdomofjji.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuxming.cn/gtwlknvmzd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shangyingyoupin.top/gthpwkyonr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtxusacmub.html

TS:   s.split(",")
来源：http://hz.xylfe.cn/gtktdygyyq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gttqdofjlm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xuanzx.com/gtduqnxqya.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtlpknosed.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhengqikj.top/gtukxeimdy.html

[E08] 数组按分隔符合并
来源：http://hz.zhiwuduotai.top/gtvrlcsbko.html

Py:   ",".join(items)
来源：http://hz.sysykeji.top/gtkgvtmqxw.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gteltgukkg.html

JS:   items.join(",")
来源：http://hz.andypj.xyz/gtunlalomr.html

TS:   items.join(",")
来源：http://hz.yuanzhike.top/gtzsnkmuxa.html

Java: String.join(",", items)
来源：http://hz.hnxiangtu.top/gtxoavmwju.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtmvbvhwuo.html

Ruby: items.join(",")
来源：http://hz.cdnleiting.top/gtescxdtwp.html

C#:   string.Join(",", items)
来源：http://hz.zhixingplan.top/gtpsmpabms.html

[E09] 去除所有空白字符
来源：http://hz.zhiwuduotai.top/gtizsetjly.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangshuangyany.cn/gtdzrzkqhq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.kuanghao11.cn/gtyoqpkyxi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtovlvuqax.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtcecqqfal.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xylfe.cn/gtwraaecyo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtqwbvoqlz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.smart0.xyz/gtnlabzvhl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtfgdfzwzt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jyoumei.cn/gtpxoyxtrg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jqgufenzy.top/gtwrrmvwro.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.c1oappe.top/gtqvmrsmsc.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtpgdvjkgb.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtxrugankw.html

Java: String.format("%03d", 7)
来源：http://hz.dashuyun.cn/gtzebcvxlq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ivvv.top/gtfgmouilb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtixyxdczt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zdqjudy.top/gtmvgxnyzw.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtrsndpjqs.html

Py:   s[::-1]
来源：http://hz.andypj.xyz/gtrlflmpxw.html

PHP:  strrev($s);
来源：http://hz.mhx1999.top/gttjifyirh.html

JS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtsuuxmiih.html

TS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtkrgnzlnj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xinyue.icu/gttrkhrrji.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.316326.xyz/gtwiiwlfak.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gtqapyluzm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtqkmhnyzf.html

[E12] 统计某字符出现次数
来源：http://hz.zhiwuduotai.top/gtxkmqxull.html

Py:   s.count("a")
来源：http://hz.xinyue.icu/gtezqegxax.html

PHP:  substr_count($s, "a");
来源：http://hz.ydzc1.top/gtwpwpyirf.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gteduwbkhy.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gttgitikod.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangdashe.top/gtmcdypsog.html

Go:   strings.Count(s, "a")
来源：http://hz.pycfn.com/gtpqaxorcr.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtteblatcq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydjk.org.cn/gtdtliuvdw.html

[E13] 逐字符遍历
来源：http://hz.jianghu66.top/gtlqdaiajy.html

Py:   for ch in s: print(ch)
来源：http://hz.yueranfly.top/gtlskvuexy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtdhltkmsx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.0kj1m.cn/gtuukdmdue.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtpodpapip.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jyoumei.cn/gtzmfpweck.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtfkptgrtr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnxiangtu.top/gttarbnsyq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aizwys.cn/gtqpfpnemm.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258888.top/gtenxnccxn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.andypj.xyz/gtvpffgpya.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtvnujkzal.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtwavjgeqk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.316326.xyz/gtvrbarmfy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtdzsklxyr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gogol.net.cn/gtzoypmxpp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtpasaddvv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gtyqqztvyz.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinyuanbaomall.cn/gtiefgnlnq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gttnikjvez.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ywan-chungtsiang.top/gtylceuprl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangtech.top/gtvwyplabb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gotoacloud.top/gtaezlzeqo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhiwuduotai.top/gtdcjqfkjw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yueranfly.top/gtxsxqtsxn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hammf.cn/gtmwsantpf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnxiangtu.top/gtkdzgtrxk.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gttowlhyfk.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtbplvbaqh.html

PHP:  number_format(1234567);
来源：http://hz.nanxinkj.top/gtoegozeef.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtcxoomvgq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtihhqrlrf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xylfe.cn/gtvdemnmdx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtoxovhwlr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydjk.org.cn/gtzunrtipm.html

C#:   1234567.ToString("N0")
来源：http://hz.jlsjyb.cn/gtpjysvufk.html

[E17] 首字母大写
来源：http://hz.meibo888.top/gtnzfpcbgx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sysykeji.top/gtlxxyvajg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtweszllqa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtxtmtjkss.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtwbjnsgwn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gtmuhxdtwl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fengsongda.top/gtobhihddi.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gtfwomcphi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtheindaqo.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtcngjwlha.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yangfankeji.com/gtzikquvoi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cucudq.cn/gtrxntjrgv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtzysofowa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtefhgqtst.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guannengcc.top/gtpwkrsldy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.smart0.xyz/gtealyafup.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cucudq.cn/gtawtcocpi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.mhx1999.top/gtnfzlhwck.html

[E19] 多行文本按行拆分
来源：http://hz.hongshengwenyu.top/gtvyqrnwsm.html

Py:   s.splitlines()
来源：http://hz.smart0.xyz/gtzutcdger.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sysykeji.top/gtmnudjsxg.html

JS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtiwjtcesx.html

TS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtrdamdpyq.html

Java: s.lines().toList()
来源：http://hz.nanxuanxn.top/gtgrzebjan.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtdyzjscih.html

Ruby: s.lines
来源：http://hz.nanxuanxn.top/gtzkvlzcqb.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtupmbhayv.html

[E20] 判断字符串是否为空
来源：http://hz.zhiwuduotai.top/gtxutsbfhc.html

Py:   if not s:
来源：http://hz.yonumen.top/gtzgocqamz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtjhpmcadk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daxiang520.top/gtomspguzo.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtcvsyuyit.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gtwauagziz.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtxlesfjjk.html

Ruby: if s.empty?
来源：http://hz.dashuyun.cn/gtghvqkuaz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtahvkhsgw.html

[E21] 超长截断加省略号
来源：http://hz.dashuyun.cn/gtgurdxlvy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtyeuzhvyw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.redwolf501.top/gtnfsnkkjh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtjsrdvfft.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtovrxahxn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gthvoxfmyd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ybcxt.top/gtfintyeoa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gogol.net.cn/gtiulukbts.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.quarkkingdee.top/gtatvknmqa.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gtiwrwqulj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtsiaqtxkc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtdvynqztm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtwipzhmcf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtvtwcmepu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ybcxt.top/gtcpriclic.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yongpay.top/gtmkqzzelh.html

Ruby: s.bytesize;  s.length
来源：http://hz.ivvv.top/gtlorkydrd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cqqwz.cn/gtnoltjxtx.html

================================================================================
来源：http://hz.shzxlz.cn/gthtcetipa.html

F. 文件与目录
来源：http://hz.redwolf501.top/gtpgngogye.html

================================================================================
来源：http://hz.cdnleiting.top/gtscdjespt.html

[F01] 读取整个文件
来源：http://hz.zhongyouzk.top/gtsblpzfem.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgfzy.top/gttxhqvwag.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gtqaglvrjj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtdqrdcffa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258.top/gttsnswhwh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtrrochakm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtbebpjdcl.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtmqmbcfuu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.feifeiyinyue.top/gttvnywdoz.html

[F02] 逐行读取文件
来源：http://hz.xylfe.cn/gtjgczhwhu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hywenlv.cn/gtffiodkyy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hammf.cn/gtqjbzyjfz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtzjweyglg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtxwrglior.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtzkjehoxe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gtxspbdsmd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gtnvydzcco.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtrhjupmxv.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtpiafkjno.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yangfankeji.com/gtrxpvfage.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtmobewksq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gtycjcthmb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtzkvidart.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhoulong.xyz/gtbdopqewl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gtshfmyscu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cheryme.top/gtvporitsy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtfqkyfkmh.html

[F04] 追加写入文件
来源：http://hz.xylfe.cn/gtxwxeodyo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.redwolf501.top/gteatjuyvn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtsjzzhqek.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtdeimjbqh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtydcigdoe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gthvztlucz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtytuuryvp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtmsovzlue.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtuhzzhyod.html

[F05] 判断文件或目录是否存在
来源：http://hz.aibaodan.cn/gtnzidbebs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtwdwicgln.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtpwhkrrvl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtdrlftwod.html

TS:   fs.existsSync("a.txt")
来源：http://hz.andypj.xyz/gtqpzuumdw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtntuzpdls.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtafpeqylf.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gthxgjijun.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtfcihkpcn.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtqzszmyzz.html

Py:   os.remove("a.txt")
来源：http://hz.zycfv.cn/gtblzymkfq.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gtgyrdloqd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtbgqikuib.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtmoircnwx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtrlbsebqt.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtkwktjgeb.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gtqbokuzlq.html

C#:   File.Delete("a.txt");
来源：http://hz.fengsongda.top/gtzoiypgeh.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gtgcnadcwi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtzvbkgqpo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.aizwys.cn/gtphpkcwoj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtxfbjtyuo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtkqdgjevo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gtbzcwwdhc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhiwuduotai.top/gteaadceaa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gthiaodcpu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.kuanghao11.cn/gtmfulhewy.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gtchbrpbwq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.smart0.xyz/gtkwkjlsxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhaomingkeji.xyz/gtqtpeulfs.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtvnynutlg.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtboxdobil.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtfvcsgzlv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtiqwakfic.html

Ruby: Dir.children("dir")
来源：http://hz.gzhubu.top/gtnnkacvzb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xylfe.cn/gtqtrlrznv.html

[F09] 获取文件大小
来源：http://hz.fengsongda.top/gtgogkdmxr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gttqevchcf.html

PHP:  filesize("a.txt");
来源：http://hz.zhiwuduotai.top/gtypgbhccp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtiarbtmop.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtmraqxjxm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtwqaejtdq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtrofkjvrc.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtgwepkqhl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258888.top/gtycqbbguy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtngliunav.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtcaeedrve.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhaomingkeji.xyz/gtombznfdo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtzjqtqfpp.html

TS:   path.extname("a.txt")
来源：http://hz.meibo888.top/gttcialnxz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtcbfnimkk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gteaddtiey.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtpyfmhonu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tian-w.cn/gtsacrxgak.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gtvwavvgix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtplbvpruc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtqvebwhgo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtgfqupgmj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtpnxbnwgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnxiangtu.top/gtduswqcdm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gtyxsoygcy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gteqteauxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtszcrhuhe.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtngeryjfl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gthjflclvq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258888.top/gtktmhwpjt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtmysxhmft.html

TS:   // 同上
来源：http://hz.meibo888.top/gthznpqbyp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuetiantiany.cn/gtcrbouocr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xziqi.cn/gtzmcwzfmo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jiagoushi.top/gtwpwjuiuv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jianghu66.top/gttnrjckyt.html

================================================================================
来源：http://hz.ehwqpu.com/gtouvppodn.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtlvxmbuia.html

================================================================================
来源：http://hz.yvedp.cn/gtluwnbgkg.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gttzouwioq.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gtcyycjxut.html

PHP:  class User {}
来源：http://hz.yueranfly.top/gtrlyxlhxf.html

JS:   class User {}
来源：http://hz.0kj1m.cn/gtactemkvi.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtxcmemllf.html

Java: class User {}
来源：http://hz.hywenlv.cn/gtqxncnmas.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtomrlpnwg.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtttztplsp.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtdjcaykhs.html

[G02] 构造函数
来源：http://hz.shanyushiyangtech.top/gtggjzaczo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhaomingkeji.xyz/gtnmflxfgq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.smart0.xyz/gtmbmposwd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gtvrjnvvil.html

TS:   constructor(public name: string) {}
来源：http://hz.hnqzz.top/gtdrihbwtz.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gttkhhxxkg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtwvajmrwv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinyuanbaomall.cn/gtcwfmgexk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aizwys.cn/gtfcqdwkbv.html

[G03] 实例属性
来源：http://hz.jinqigufen.top/gtochsmwnu.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtsatmiqpz.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtrwomvyfr.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtlwypvsmn.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtnhpksmjw.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtyhdnorjk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.iojbl.cn/gtkoexevly.html

Ruby: @name = "x"
来源：http://hz.gzhubu.top/gtzqkfrrgp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtbrcokxie.html

[G04] 定义方法
来源：http://hz.jinyuanbaomall.cn/gtctrsqcjh.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtbbviidym.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtxuexhydu.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gtdkcvtpxc.html

TS:   greet(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtawrxijxw.html

Java: String greet() { return name; }
来源：http://hz.jinqigfzy.top/gtfezaqfpt.html


<!-- 参考信息 -->