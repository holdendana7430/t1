代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.mhx1999.top/gtyktuxysb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.birdmap.top/gtuymynnef.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gtstyhjbtp.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtcmvbkown.html

PHP:  implode(",", $items);
来源：http://hz.zhongyouzk.top/gtygsvglwf.html

JS:   items.join(",")
来源：http://hz.cucudq.cn/gtoawakoih.html

TS:   items.join(",")
来源：http://hz.gzhubu.top/gtumqcbyla.html

Java: String.join(",", items)
来源：http://hz.aibaodan.cn/gtcmkengrp.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtdgjfblhl.html

Ruby: items.join(",")
来源：http://hz.cqqwz.cn/gtwwdlopdh.html

C#:   string.Join(",", items)
来源：http://hz.dashuyun.cn/gtwhuywaua.html

[E09] 去除所有空白字符
来源：http://hz.hfpthk.cn/gtkoeeplyw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daxiang520.top/gtlhillbsy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jlsjyb.cn/gtzgswxvbf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinghuilouyu.cn/gtokumjjlw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtvdogqfyh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxinkj.top/gtypxracsi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtrfikcvtb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cheryme.top/gttlyussfy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.birdmap.top/gthpdvzdpm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtuunyvwsw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtrcumnpao.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigufen.top/gtjzmjuyeg.html

JS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtgaskluzy.html

TS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtzaaqmubb.html

Java: String.format("%03d", 7)
来源：http://hz.smart0.xyz/gtgmauzldd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtrjfummct.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtazahrpux.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gtvbokmsqz.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtjseagijw.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gtfvnhzbij.html

PHP:  strrev($s);
来源：http://hz.fengsongda.top/gtpmxqiedu.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtndqdywsz.html

TS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtcjgpfflh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tianlin.xyz/gtamrdcqlu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.meibo888.top/gtpchjlaer.html

Ruby: s.reverse
来源：http://hz.guowangkeji.top/gtclcktanr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtpxmnjcfj.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gtouuhjdjx.html

Py:   s.count("a")
来源：http://hz.sysykeji.top/gtuqgaqhyq.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtfadsyaew.html

JS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtbacxgqzz.html

TS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtaogopcol.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhengqikj.top/gtfxxreqpw.html

Go:   strings.Count(s, "a")
来源：http://hz.yangfankeji.com/gtgkazrvxk.html

Ruby: s.count("a")
来源：http://hz.tianlin.xyz/gtyjgoysxo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jianghu66.top/gtxafmgntt.html

[E13] 逐字符遍历
来源：http://hz.wangdashe.top/gtcoizegce.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtozxqrcdd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenjidiqi.icu/gttczqgpyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtsvbqzosv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gthqxfuoqz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ivvv.top/gtgwbxwwgq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.andypj.xyz/gtoaxqvnyw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fengsongda.top/gtxemzdjpq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gthucapqvy.html

[E14] URL 编码与 Base64
来源：http://hz.yueranfly.top/gtzxvalzfe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gthanjgjqg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.redwolf501.top/gtyhakuqfv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jlsjyb.cn/gtasqzoemy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sufxvd.cn/gtasxwcoyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.smart0.xyz/gtbczllzwc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtjgqvbegg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtfhytfpxv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhaomingkeji.xyz/gtgykymsqi.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtbyjyrckd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtzszfcbch.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydjk.org.cn/gtllmcvadm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gttrzczlyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtvfqzwpmt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtkxozpvio.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guowangkeji.top/gtblcfrlhq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fzhhl.top/gtighkymiq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.9152youxi.cn/gtijtkvsdj.html

[E16] 数字千分位
来源：http://hz.sweek.top/gtucnfanil.html

Py:   f"{1234567:,}"
来源：http://hz.yueranfly.top/gtgmfhdnfj.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gtrguqfbhr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtfanhkygv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtysipqluh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.0kj1m.cn/gtujgdnlfh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hysaishi.cn/gtwenqsbtn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gtgrhcispz.html

C#:   1234567.ToString("N0")
来源：http://hz.hywenlv.cn/gtkkqvoezu.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtoubxgaoq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yueranfly.top/gtjjuzzovg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.meibo888.top/gtubnmtvnc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtjdkrquno.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtnbfqnitn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gtevbyarlo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuxming.cn/gtuchqulsy.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtdbeaslyw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtsxgubwsb.html

[E18] 模板占位符替换
来源：http://hz.ywan-chungtsiang.top/gthooxdlux.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tianlin.xyz/gtmyukdact.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtsigvfzbe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gtjyuayvyj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gttrovokpo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhixingplan.top/gthjzjixto.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtdeczwakj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtfteboyol.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fzhhl.top/gtiuxksieo.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtlvyubgtx.html

Py:   s.splitlines()
来源：http://hz.redwolf501.top/gtvrwxmzks.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuanzhike.top/gtptjzdzlx.html

JS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtoochxiym.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtdvtarvkz.html

Java: s.lines().toList()
来源：http://hz.9152youxi.cn/gteefcubyr.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gtwnigjfib.html

Ruby: s.lines
来源：http://hz.yj20258.top/gtbxqmpwik.html

C#:   s.Split('\n')
来源：http://hz.zhaomingkeji.xyz/gtbcmivfpo.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtjtucyirf.html

Py:   if not s:
来源：http://hz.yj20258.top/gtdsuwaiwq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gthmabygtx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xinyue.icu/gtufzaufvf.html

TS:   if (s === "") {}
来源：http://hz.dianchejie.cn/gtmmvmtskh.html

Java: if (s.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtxbsjieju.html

Go:   if s == "" {}
来源：http://hz.kuanghao11.cn/gtcdajiere.html

Ruby: if s.empty?
来源：http://hz.yuxming.cn/gtvfdmeqqb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenjidiqi.icu/gtdkykvbbj.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtjldhcllc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zdqjudy.top/gtidpqtfgb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtojocuizw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtyydxcris.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtdxclusam.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtqxfpyhcb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxuanxn.top/gtnwzxvjpg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gaohongyu789.top/gtnnlgybgw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtcitwhgex.html

[E22] 字节长度与字符长度
来源：http://hz.hnqzz.top/gtfktunzta.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtruewsceu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtwfpavcpe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtxamxtquf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtxzujsovn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tanke756.top/gtlcjlbeqv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuanzhike.top/gtwbtdtzgg.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtqhivbsxc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtdugejjkt.html

================================================================================
来源：http://hz.ivvv.top/gtlrmhauut.html

F. 文件与目录
来源：http://hz.cashguo.top/gtlhthvlfw.html

================================================================================
来源：http://hz.gogol.net.cn/gtaodebdom.html

[F01] 读取整个文件
来源：http://hz.yuxming.cn/gtzuzmiflc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtnzjnvehg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtphohzqky.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtrqccjgys.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shuidangran.top/gtindejwiw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtgqcnmexf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxinkj.top/gtvzeelawa.html

Ruby: File.read("a.txt")
来源：http://hz.xuetiantiany.cn/gtjsghmkkd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hammf.cn/gtmbezxrxl.html

[F02] 逐行读取文件
来源：http://hz.aizwys.cn/gtlhtezpps.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuetiantiany.cn/gtgiuzxmyd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtklppmnsu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gtcpiwjxlm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtrolxffow.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtpfdvsaqm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtzvzihepy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtogktnfhn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.haohaochexian.top/gtmnxwdtjh.html

[F03] 写入文件（覆盖）
来源：http://hz.ydjk.org.cn/gtibbscelj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tian-w.cn/gtxbrujxns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangkeji.top/gtacwwpjzh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtjzumuzas.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtpaaohoua.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtwjqrohks.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtpirgemsf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tanke756.top/gtnftljxzo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtglxcbajj.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtdutnxshk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yongpay.top/gtwprdnien.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtcmbqibnh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtqgspuoiu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtqnzhkcik.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnqzz.top/gtvzqmxrrq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hfpthk.cn/gtjglvfnmc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xylfe.cn/gtyxataafg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dashuyun.cn/gtvnewnxnf.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gtckvecmrs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xylfe.cn/gtrnbdukis.html

PHP:  file_exists("a.txt");
来源：http://hz.haohaochexian.top/gtfutdahzw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtxzovpeye.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtjcqrsera.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtlpjbcxve.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtyknuikbz.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuanzx.com/gtjabvxrou.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtphihvspe.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtlzvudsiy.html

Py:   os.remove("a.txt")
来源：http://hz.cucudq.cn/gtmdhtmkys.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtklavcefs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtacfxjsqb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtyxzdejeu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtexpuofzo.html

Go:   os.Remove("a.txt")
来源：http://hz.hnxiangtu.top/gthyrfatvt.html

Ruby: File.delete("a.txt")
来源：http://hz.quarkkingdee.top/gtaegwdpsh.html

C#:   File.Delete("a.txt");
来源：http://hz.hammf.cn/gtqhnnugcd.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtpjhwgcjs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sufxvd.cn/gtpouubzlk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtismkpqoo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtiidldtus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtqkciqgkt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ivvv.top/gtznobocqi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yongpay.top/gtgebbievc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtiuelsrdz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yangfankeji.com/gtwevurtbt.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtgbsfeqyl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhaomingkeji.xyz/gtdlbhggio.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtqximmpic.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtgjbvrqhe.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtnkbecrnv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtgnenhisg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ehwqpu.com/gtcwbjtihu.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtmfozvtcr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtaljvutry.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtfqdxkxmt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtjqnyuxac.html

PHP:  filesize("a.txt");
来源：http://hz.tianlin.xyz/gtzgxyszdt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtagwelubi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtnkfaczrj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtzesbbzld.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtozbnbbog.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtahtwmfap.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangtech.top/gtglizrvhl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtdflldhfk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtzuknftlv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxuanxn.top/gtdkhikyzm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtmxjfozdr.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtrhqjoryc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtjmlrjvou.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtvxzcnxpn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtxzlyvwis.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dashuyun.cn/gtacvdqpvs.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gthavnqeuv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtlzwpmvyu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hammf.cn/gtnxvawsay.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtgucjxkes.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtyuoimhjw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guannengcc.top/gtajtuuwyt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hongshengwenyu.top/gtcmzessna.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtqkhvjthf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtwdcugxcl.html

[F12] CSV 读写
来源：http://hz.cqqwz.cn/gtiqfukczy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gthkjcdqxi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtmpnrpmja.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.bjfxy.top/gtsobseajf.html

TS:   // 同上
来源：http://hz.cheryme.top/gtibioavce.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnqzz.top/gtxdnxlmmh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aizwys.cn/gtliimaqll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtzolyuebf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fengsongda.top/gtqzccoqtr.html

================================================================================
来源：http://hz.zdqjudy.top/gtaymnffio.html

G. 面向对象
来源：http://hz.jinqigfzy.top/gtvqmuqbkv.html

================================================================================
来源：http://hz.yj20258888.top/gtkrswirag.html

[G01] 定义类
来源：http://hz.pycfn.com/gtxhnfpvmi.html

Py:   class User: pass
来源：http://hz.yongpay.top/gthivatnjf.html

PHP:  class User {}
来源：http://hz.smart0.xyz/gtdxrmjrug.html

JS:   class User {}
来源：http://hz.shangyingyoupin.top/gtwssezarn.html

TS:   class User { name: string = ""; }
来源：http://hz.wangdashe.top/gteosacwow.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtbzclwtmo.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gttanztapn.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtyluctcat.html

C#:   class User {}
来源：http://hz.yongpay.top/gtdwrcjqcs.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtbpzalzfq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtlcgzbpdx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtztcodjax.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtaexcbfnj.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtxparcwbi.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtnadsuudx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuanzx.com/gtcxsucbdu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.quarkkingdee.top/gtgbglhllx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dianchejie.cn/gtidtctxsy.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtqjhvqzun.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtwcvjvqwf.html

PHP:  public string $name = "x";
来源：http://hz.9152youxi.cn/gtgnjrlohy.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtqktwyfyg.html

TS:   name: string = "x";
来源：http://hz.iojbl.cn/gtgagsqvth.html

Java: private String name;
来源：http://hz.ppjwa.cn/gtytfsfvnb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jlsjyb.cn/gtmvysnhlf.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtxdxbmhns.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtmtxvhxoj.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtzqhbvagm.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gttkxpflfh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtreyprbin.html

JS:   greet() { return this.name; }
来源：http://hz.sysykeji.top/gtmaqqzjag.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtileohiyq.html

Java: String greet() { return name; }
来源：http://hz.guowangkeji.top/gtjbdcufqy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cheryme.top/gtmndqxtsz.html

Ruby: def greet; @name; end
来源：http://hz.chenzaomai.com/gtarfhcthc.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gtsrehlxri.html

[G05] 继承
来源：http://hz.cqqwz.cn/gtsjzmibmj.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtzewvzjgi.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtninbuyhm.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtwcnbvqht.html

TS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtlulxbsdj.html

Java: class Admin extends User {}
来源：http://hz.nanxinkj.top/gtzlaafxky.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tianlin.xyz/gttavsdrxa.html

Ruby: class Admin < User; end
来源：http://hz.sweek.top/gtfuyonlqp.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtiaierzib.html

[G06] 重写方法
来源：http://hz.xuanzx.com/gtnvhhaato.html

Py:   def greet(self): return "admin"
来源：http://hz.cheryme.top/gtpdkfxujz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtfixcmfmp.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtitqxxqdp.html


<!-- 参考信息 -->