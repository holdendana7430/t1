代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gtueunkxxp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgfzy.top/gtqmwztesr.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtetadekxk.html

Py:   ",".join(items)
来源：http://hz.chenzaomai.com/gtgktugxuk.html

PHP:  implode(",", $items);
来源：http://hz.gaohongyu789.top/gtmryxeqke.html

JS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtvirgijex.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtzmxztolh.html

Java: String.join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtykxeowqc.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtecvzamsd.html

Ruby: items.join(",")
来源：http://hz.nanxinkj.top/gtvjinkvlv.html

C#:   string.Join(",", items)
来源：http://hz.ywan-chungtsiang.top/gtwulvzjut.html

[E09] 去除所有空白字符
来源：http://hz.hfpthk.cn/gtubgrkhen.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtcnyawhbv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hfpthk.cn/gtrsqqcqmj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtqgccvntx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtmougasyo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gtqdddhtov.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hfpthk.cn/gtdvhedird.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zycfv.cn/gtftxvxxvf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtlgdwrvlb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtwrzlmgqb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj20258888.top/gtnlmbbmck.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtoiabwxqi.html

JS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtulmznfxk.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj202588.top/gtlfblctxg.html

Java: String.format("%03d", 7)
来源：http://hz.yuxming.cn/gtepxczrup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cucudq.cn/gtncydvaoq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fengsongda.top/gtklpikfzm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ppjwa.cn/gtwydisjvs.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtfsssjqxm.html

Py:   s[::-1]
来源：http://hz.c1oappe.top/gtjqdqyrjp.html

PHP:  strrev($s);
来源：http://hz.ehwqpu.com/gtothlxxpj.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtqrdnwjic.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtrzpvvdjz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gthgqbnsvz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gtfsnwdrww.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtiltwtpwt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ppjwa.cn/gtulpmxasx.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangkeji.top/gtrnbysgih.html

Py:   s.count("a")
来源：http://hz.c1oappe.top/gtnntxrhxw.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtcxinaofn.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtdvryuwso.html

TS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gtyhxkfouc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxinkj.top/gtaesmppyb.html

Go:   strings.Count(s, "a")
来源：http://hz.zhiwuduotai.top/gtetckooir.html

Ruby: s.count("a")
来源：http://hz.haohaochexian.top/gtopkcnasz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258.top/gtvuvawdaz.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtrjyqffcl.html

Py:   for ch in s: print(ch)
来源：http://hz.xuanzx.com/gtoywmxqzv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shuidangran.top/gtwrgnedqv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtyjiyzdzr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtnjfapbht.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangkeji.top/gtnzjqrqpe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cqqwz.cn/gtjzecqvvr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj202588.top/gtdnznsvnh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xylfe.cn/gtwojwehcu.html

[E14] URL 编码与 Base64
来源：http://hz.smart0.xyz/gtgroavjnj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhijiandao.cn/gtkfztdkli.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtsjjkyefy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jyoumei.cn/gtzibkuala.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.smart0.xyz/gtlibjjrbm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydzc1.top/gtlprfantu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtlcdbqago.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gaohongyu789.top/gtcrbrhlnu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.nanxinkj.top/gttqicmtjg.html

[E15] HTML 转义 / 反转义
来源：http://hz.aizwys.cn/gtozrasipv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gtsnzwejqx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.quarkkingdee.top/gtpbdwcaxl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhengqikj.top/gtuzhifchm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtkzvoghue.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cdnleiting.top/gtyzlbiowk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sxryk.cn/gtpnqbsvgr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cqqwz.cn/gtaedsjhdi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shzxlz.cn/gtktgwaqdd.html

[E16] 数字千分位
来源：http://hz.fengsongda.top/gtzpmfosxz.html

Py:   f"{1234567:,}"
来源：http://hz.ehwqpu.com/gtatioarqp.html

PHP:  number_format(1234567);
来源：http://hz.hfpthk.cn/gtxflzfwif.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtactejyog.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtnaodnqvo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhengqikj.top/gteokzxbux.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gtdnwqiquy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.havefunace.top/gtzqbttdpv.html

C#:   1234567.ToString("N0")
来源：http://hz.ybcxt.top/gtopexqeuo.html

[E17] 首字母大写
来源：http://hz.daria6918.cn/gtelqiuzvg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.9152youxi.cn/gtblxbfatr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtyeqiwvwp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtqyyxkfrt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtphezxwel.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtdejyvgtz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cdnleiting.top/gthugsqwah.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gttfxkhddo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hnxiangtu.top/gtxywttzmm.html

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gtlqbagurt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhengqikj.top/gtghtvpvat.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtzabbtefh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtzydhytbj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtgmjnzhev.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tanke756.top/gtvrhbxrbj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.redwolf501.top/gtdwvrznhx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.kuanghao11.cn/gtwpfyvejc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtkezktulr.html

[E19] 多行文本按行拆分
来源：http://hz.nwbrower.top/gtxwqtvibu.html

Py:   s.splitlines()
来源：http://hz.52xcode.cn/gtyqoicmgv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgufenzy.top/gtnmaqxxsz.html

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtzprmkzmj.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtrpkjfxec.html

Java: s.lines().toList()
来源：http://hz.dashuyun.cn/gtfehgjerp.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuetiantiany.cn/gtnlmngdtx.html

Ruby: s.lines
来源：http://hz.jqgufenzy.top/gtkklpcaej.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtgojolwtq.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gtytbjqrfs.html

Py:   if not s:
来源：http://hz.smart0.xyz/gtwwppxxba.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtcwuphwdz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daxiang520.top/gtydxnpeou.html

TS:   if (s === "") {}
来源：http://hz.jinqigfzy.top/gtspzmfjxu.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258888.top/gtvmsjesjf.html

Go:   if s == "" {}
来源：http://hz.vqdsnc.cn/gtkuorlqkb.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtsdhqgqia.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jlsjyb.cn/gtwaixzzda.html

[E21] 超长截断加省略号
来源：http://hz.cheryme.top/gtzmyldayr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtlkqwhhdd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dianchejie.cn/gtrytlvjug.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtchdpjtgy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtytzjvlcx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtgmwkbsyu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtccdbgxiz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.redwolf501.top/gtvhoegees.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtnheybymp.html

[E22] 字节长度与字符长度
来源：http://hz.yangfankeji.com/gtpqkkgfre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gtspmjwwcz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtblugpyqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtfznlrqwe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtmdwtirkh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gteaeouqly.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuxming.cn/gtseykzuqz.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtgtkvzemf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.9152youxi.cn/gtxuukpixx.html

================================================================================
来源：http://hz.gotoacloud.top/gtzbqzrowp.html

F. 文件与目录
来源：http://hz.tanke756.top/gtobdszflv.html

================================================================================
来源：http://hz.ydjk.org.cn/gtykbuafyz.html

[F01] 读取整个文件
来源：http://hz.jlsjyb.cn/gtrblbnrla.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.havefunace.top/gthlqnjmuf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtmyyyetyt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhongyouzk.top/gtpjzautfc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtdfwcxkod.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtpmujhnfn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtddpwtpcu.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtagahztml.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gtwyxlbnaj.html

[F02] 逐行读取文件
来源：http://hz.meibo888.top/gtjjhrevec.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtoqlhlwuq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zycfv.cn/gtpqavzriq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtsrjngrrq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtsjdqbxej.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtmxjfdxwp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ivvv.top/gtvxlousvi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.quarkkingdee.top/gtdnzvrtrc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtegmjrhqs.html

[F03] 写入文件（覆盖）
来源：http://hz.cheryme.top/gtyhlyxpqn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtnrnqamyb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtygysynjy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtmrcitolz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtlboucysj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gtapnragkm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.kuanghao11.cn/gtgghiuzyn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gogol.net.cn/gtavpesfil.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtaykdwuun.html

[F04] 追加写入文件
来源：http://hz.zhoulong.xyz/gtpdnyzxpd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pycfn.com/gthckaptbl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pycfn.com/gtzevuwepc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sweek.top/gtzpydkjfz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtvkdnbuwr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtfbkwysko.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtuwfevyil.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tianlin.xyz/gtilondoyx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnxiangtu.top/gtophilrvz.html

[F05] 判断文件或目录是否存在
来源：http://hz.ywan-chungtsiang.top/gtbtfajxsy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgufenzy.top/gtrdxecphd.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtijejxlze.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtzxkoejrs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtbkjpafom.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtnkqhfxkr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zycfv.cn/gtfbwlpxvp.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtknqxwsey.html

C#:   File.Exists("a.txt")
来源：http://hz.yuxming.cn/gtuthwfupz.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtscairefn.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtbsmnyjnt.html

PHP:  unlink("a.txt");
来源：http://hz.shangyingyoupin.top/gtolkjuygm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtmcwczldw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtydfsqbpd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtwpjrlzsv.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtfeaqdayy.html

Ruby: File.delete("a.txt")
来源：http://hz.jyoumei.cn/gtrvkiixcu.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtiashiiqm.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtkylcaslg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dashuyun.cn/gtewhgjcof.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtwfgkkdtk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtuyzofkex.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtscdileoq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtazensjvr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zycfv.cn/gtcnipiyqr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtgjwjnzzf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtwxtrjtaq.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtbwaqrrnp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shangyingyoupin.top/gtwgxfphnl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gtflltcwmq.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gthkkkegyp.html

TS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtwslhhqhx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtrmvukvat.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gttzvfkgnc.html

Ruby: Dir.children("dir")
来源：http://hz.zhijiandao.cn/gtsxqbnbzk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xylfe.cn/gtywbpgjly.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtfnmduaus.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cqqwz.cn/gtladkmlnw.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtbhixlyag.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtmpmpnzbz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gtlehnhdrl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtmzdloore.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daxiang520.top/gtkfipmqik.html

Ruby: File.size("a.txt")
来源：http://hz.jiagoushi.top/gtaaatxobs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gaohongyu789.top/gtmcqfolun.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tian-w.cn/gttvfpkwfg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtcitejece.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gogol.net.cn/gtfzgfjlxy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gthhwxvhyw.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtgqgqnxlt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zycfv.cn/gtmmmalpjk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtzktizaqg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sweek.top/gtobpjtbmc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gttexgiowv.html

[F11] 复制与移动文件
来源：http://hz.shzxlz.cn/gtmwsfpive.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtvyapmjsd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydzc1.top/gtlpivqnvu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtsxznrafm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtoxzzafbh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cashguo.top/gtfthpfdkq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtfauzcaat.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtuspaiwql.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gtkowxnuka.html

[F12] CSV 读写
来源：http://hz.daria6918.cn/gtwewwoatj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gogol.net.cn/gtwqtyiruv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtogsluvcq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gteigvzjxz.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtkggzxrlu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtexzrbapt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtjnlulfjv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtvecdcwer.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jyoumei.cn/gtwdtxvhmr.html

================================================================================
来源：http://hz.yuxming.cn/gtuvfujsip.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtowaadlfn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgwwcgyli.html

[G01] 定义类
来源：http://hz.sufxvd.cn/gttywabpgs.html

Py:   class User: pass
来源：http://hz.yongpay.top/gtjbzvqrkh.html

PHP:  class User {}
来源：http://hz.daxiang520.top/gtuweeybxk.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gtqalkjyih.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtuvnjkpej.html

Java: class User {}
来源：http://hz.yvedp.cn/gtlrqyhmfa.html

Go:   type User struct { Name string }
来源：http://hz.hysaishi.cn/gtzsbghyay.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtotgyrgnp.html

C#:   class User {}
来源：http://hz.xziqi.cn/gtjbwuocjs.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtnwdzygcw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gtichgjnfw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtbmwjuzio.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtifxcjrnd.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtmpfmwrlv.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtbmnetehk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtonftpdmf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gtsnfnngnk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258.top/gtrpmxlcqy.html

[G03] 实例属性
来源：http://hz.daria6918.cn/gtslcibsbr.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gteuytidvg.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gtxzeezrvz.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gthtdyomwo.html

TS:   name: string = "x";
来源：http://hz.yj202588.top/gtgoiccyzj.html

Java: private String name;
来源：http://hz.tanke756.top/gtwqiwhdrj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hysaishi.cn/gtbsxcxzci.html

Ruby: @name = "x"
来源：http://hz.52xcode.cn/gtnfsracvy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fengsongda.top/gtdusbpfhn.html

[G04] 定义方法
来源：http://hz.quarkkingdee.top/gtwzpfutbs.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtwcryewuu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cashguo.top/gtggkmbqzk.html

JS:   greet() { return this.name; }
来源：http://hz.jyoumei.cn/gtuqqjnwbt.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtisksjhhy.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtcsclgvex.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gthairkelt.html

Ruby: def greet; @name; end
来源：http://hz.c1oappe.top/gtdavsqryy.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtkjvngjzk.html

[G05] 继承
来源：http://hz.svipenyu.cn/gtklaceoav.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gtcveicjbj.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtaygpxawk.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtzkkdlmvx.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtxnhojtwm.html

Java: class Admin extends User {}
来源：http://hz.gogol.net.cn/gtqxjoapni.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtfizgphik.html

Ruby: class Admin < User; end
来源：http://hz.shuidangran.top/gtajxudnbe.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtjzklsptr.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gtrdhvnfcw.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtzlamfbcl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtbbrojkht.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtmybsjhfn.html


<!-- 参考信息 -->