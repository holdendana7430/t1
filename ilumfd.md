代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.jiagoushi.top/gtiqucdqip.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgufenzy.top/gtgrtuwrqa.html

[E08] 数组按分隔符合并
来源：http://hz.chenjidiqi.icu/gtdqxjuydv.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gtntmbvhgm.html

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gtundsbzsk.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gtshzmjuor.html

TS:   items.join(",")
来源：http://hz.tian-w.cn/gtihlsqkss.html

Java: String.join(",", items)
来源：http://hz.tianlin.xyz/gtgrzsbcwy.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtbfeytqtz.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gtqhcxpdxn.html

C#:   string.Join(",", items)
来源：http://hz.wangdashe.top/gtdlcrektp.html

[E09] 去除所有空白字符
来源：http://hz.guannengcc.top/gtcolrqlkd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ybcxt.top/gtvmviggqu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gthzefpokl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtwuroxkzm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtwvpjqcdj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtrtjgiirp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgfzy.top/gthueflbme.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtuyjysxiq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tian-w.cn/gtlfjvzsgs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gogol.net.cn/gtopxkunqw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gtcefztjsl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gtgoppvqvu.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtgbqpqgpk.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangdashe.top/gtublngsxu.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtmovpsjzx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtpnxunabr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zycfv.cn/gthsfqcyrr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yanxiufei.cn/gtlhlijahd.html

[E11] 反转字符串
来源：http://hz.yj20258888.top/gtkxvjbcft.html

Py:   s[::-1]
来源：http://hz.guannengcc.top/gtjjejrhjk.html

PHP:  strrev($s);
来源：http://hz.yueranfly.top/gtxvuugicp.html

JS:   [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtslaysonv.html

TS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtzyuksgpq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zycfv.cn/gtymglneob.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtzwegfjyv.html

Ruby: s.reverse
来源：http://hz.zhiwuduotai.top/gtfwjyisay.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtijblzjze.html

[E12] 统计某字符出现次数
来源：http://hz.52xcode.cn/gtriccnjxj.html

Py:   s.count("a")
来源：http://hz.cashguo.top/gtstcefsji.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtjnnhsmig.html

JS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtzggbkuek.html

TS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtdyacvlal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtxlceakld.html

Go:   strings.Count(s, "a")
来源：http://hz.zhixingplan.top/gtxazikdpj.html

Ruby: s.count("a")
来源：http://hz.gzhubu.top/gtlmwyzcem.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ybcxt.top/gtajgighrk.html

[E13] 逐字符遍历
来源：http://hz.yuanzhike.top/gtcrhsvyrn.html

Py:   for ch in s: print(ch)
来源：http://hz.xuetiantiany.cn/gtcqmjfnnz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xylfe.cn/gtaepknwbu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtjypvvwao.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtmzeyxhgl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinghuilouyu.cn/gthccarrzo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtzdgrvxmk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.iojbl.cn/gtcgacuahy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yvedp.cn/gtaqsinyhn.html

[E14] URL 编码与 Base64
来源：http://hz.guannengcc.top/gtvfcpmivs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenzaomai.com/gtrqvaasgu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guannengcc.top/gtgzkmfbsu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtpaefqucq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtsojtcdcv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hongshengwenyu.top/gtsnuspmaq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtwkkvswxt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nanxuanxn.top/gtlhzywnfl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fengsongda.top/gtuyufshxk.html

[E15] HTML 转义 / 反转义
来源：http://hz.tianlin.xyz/gtfwvoxtmm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtlmpykmbr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.c1oappe.top/gtarmnlkil.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhaomingkeji.xyz/gtguwdjssi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuanzhike.top/gtqijnmwsk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.mhx1999.top/gtuoehesge.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.iojbl.cn/gtmnyfsebj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtqslqnvgf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhijiandao.cn/gtpfgunzsv.html

[E16] 数字千分位
来源：http://hz.jyoumei.cn/gtrygleltj.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtvxvsjjpu.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gthiwcxcpb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtejqvafng.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtfdegzxfn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aizwys.cn/gthbhxuhpf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gttjshtept.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtsnbphgsx.html

C#:   1234567.ToString("N0")
来源：http://hz.jyoumei.cn/gtgzipmvax.html

[E17] 首字母大写
来源：http://hz.9152youxi.cn/gtuzbxtglp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinghuilouyu.cn/gtidgxkcwn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuanzx.com/gtwuymjhcl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtzemrxruc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtbcjakknf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guowangkeji.top/gtutjrpbns.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ivvv.top/gtdeptevcr.html

Ruby: s.capitalize
来源：http://hz.haohaochexian.top/gtknybahxp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.0kj1m.cn/gtkfanckpl.html

[E18] 模板占位符替换
来源：http://hz.jyoumei.cn/gtnqpgluuc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nanxuanxn.top/gthbwersof.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtivcejkym.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtayystuju.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtxzddcwyq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shzxlz.cn/gtuoquevgg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtqzhcxkpt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.svipenyu.cn/gthcmjwtni.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shuidangran.top/gtstjhgyfn.html

[E19] 多行文本按行拆分
来源：http://hz.snrcjt.cn/gttphkdyid.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gttxbuhbpa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zycfv.cn/gtvhddutjp.html

JS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtaitzppnm.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtytjzlcba.html

Java: s.lines().toList()
来源：http://hz.ydzc1.top/gthxxvhcxg.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtpfoaehiy.html

Ruby: s.lines
来源：http://hz.shzxlz.cn/gtkbfpunpr.html

C#:   s.Split('\n')
来源：http://hz.yuxming.cn/gtmefjjelc.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gteubnesse.html

Py:   if not s:
来源：http://hz.chenjidiqi.icu/gtsvytatdw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtjbedcaci.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.meibo888.top/gtrszsgykp.html

TS:   if (s === "") {}
来源：http://hz.bjfxy.top/gtvveeohut.html

Java: if (s.isEmpty()) {}
来源：http://hz.shuidangran.top/gtfmvymcdr.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtcylbzupe.html

Ruby: if s.empty?
来源：http://hz.gogol.net.cn/gtgedxszfl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nwbrower.top/gthnquicme.html

[E21] 超长截断加省略号
来源：http://hz.c1oappe.top/gtvwmtaguf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ehwqpu.com/gtitvzlyff.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gttyefmhwr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtbozvhunv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtqvfbcpqr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtjauzcelt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gticckrnyr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtmofqllnd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gtvlbubmhu.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtkuostgbj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.0kj1m.cn/gtidibmtkw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtpnbgcszq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gthymaojrn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtedtxhbyy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gtegizrudy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gtwwcyeifq.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtihlzhsia.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gtkvffqkje.html

================================================================================
来源：http://hz.yanxiufei.cn/gtuwwujzya.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtuwnjzdzy.html

================================================================================
来源：http://hz.haohaochexian.top/gtmcsygzbj.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gtziwloujm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gttcqjuvjz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sufxvd.cn/gtezsexady.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cheryme.top/gtqhqdugtd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jyoumei.cn/gtudpiuqlc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtnkzztlfr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hfpthk.cn/gtdaoxaoiy.html

Ruby: File.read("a.txt")
来源：http://hz.gotoacloud.top/gthesxmjff.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gtrkgaxlpg.html

[F02] 逐行读取文件
来源：http://hz.xingfuxueyuan.xyz/gtqmkbmuqo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gttmeowksq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258.top/gtgtiarhdj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gthlcklrgq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtcqzwcfzm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtowkgbkki.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtafnakyzt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtpcrosdph.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yueranfly.top/gtjupqredk.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtxffdjmek.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gaohongyu789.top/gtvxmiqayz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gtizsoajkb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtglwisfml.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtqhtbaghb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtlwzdrsvb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gtnnymabeh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.svipenyu.cn/gtxtzugrra.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtckkqmjca.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gtznwnadup.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sxryk.cn/gtfucbvbkk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtuthriiof.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtoavwtops.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtnkmmfjaz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtzcqlfpoe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtixkxgekz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtbyypcqcb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtxusksewr.html

[F05] 判断文件或目录是否存在
来源：http://hz.dashuyun.cn/gtgdovjutb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ywan-chungtsiang.top/gtvhfaqhve.html

PHP:  file_exists("a.txt");
来源：http://hz.fengsongda.top/gtydthuegm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtzrunyrzy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtgwmbkecx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtozbxxbci.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtpxopuybi.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtiecgvosn.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtcegpizlh.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gthxmieveq.html

Py:   os.remove("a.txt")
来源：http://hz.aibaodan.cn/gtzsxgmaiw.html

PHP:  unlink("a.txt");
来源：http://hz.feifeiyinyue.top/gtdyoflpqn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtuqsoizch.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtptwcdach.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtfqohjhny.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtjehomtzf.html

Ruby: File.delete("a.txt")
来源：http://hz.quarkkingdee.top/gthrcomqzw.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gtorgeqaub.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtgtompdca.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.c1oappe.top/gtferuejsd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.birdmap.top/gtgjalwzib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtibotyveg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtuiginril.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtgmzfqvxc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtgnkktoqe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dashuyun.cn/gtwfombbhs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtsuxamyuf.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gtrmaukdgj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gtddpxlbcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtgsrlpzds.html

JS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtdxbaygbz.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtgwapndkg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtljxyecoq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gtfejspizm.html

Ruby: Dir.children("dir")
来源：http://hz.c1oappe.top/gttssxoapx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ydzc1.top/gtggthhdag.html

[F09] 获取文件大小
来源：http://hz.fengsongda.top/gtvxhavwps.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtdxgnndli.html

PHP:  filesize("a.txt");
来源：http://hz.ydzc1.top/gtcmvtchmj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtfhpcdqtb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtbtywvjcf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtbqghxuem.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenzaomai.com/gtxirnnlsc.html

Ruby: File.size("a.txt")
来源：http://hz.cheryme.top/gtjkundoql.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aizwys.cn/gtcqrabbhs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gtlbandvxc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtuvcymezb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtkybvfnrf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtmzjvuypt.html

TS:   path.extname("a.txt")
来源：http://hz.chenjidiqi.icu/gtugheguwv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gtlcclvpez.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtgykgrxtt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtznfgkrjj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yonumen.top/gtzbflnwth.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtezsieioc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtspybzmqj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cheryme.top/gtiihjpxxz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtrndmflfc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtzvftpfrq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtmjneneza.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtkxzqlcyv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtzuguhzdf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtaslmohqk.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtzljtfson.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtgguliffk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gturyuefoq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtctzcebzv.html

TS:   // 同上
来源：http://hz.smart0.xyz/gtaupxorxk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shangyingyoupin.top/gteumsjiyp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gtcotcxxma.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtyhawlqze.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenjidiqi.icu/gtynpqjkdb.html

================================================================================
来源：http://hz.sxryk.cn/gtgosjekbb.html

G. 面向对象
来源：http://hz.hywenlv.cn/gtxxnvirkf.html

================================================================================
来源：http://hz.dashuyun.cn/gtofpbeszu.html

[G01] 定义类
来源：http://hz.yueranfly.top/gtzgljwlxm.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtezsxhlci.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gteoxxtjfo.html

JS:   class User {}
来源：http://hz.yvedp.cn/gtrmkqduka.html

TS:   class User { name: string = ""; }
来源：http://hz.hywenlv.cn/gtnuuwaiqj.html

Java: class User {}
来源：http://hz.yvedp.cn/gtebyeirkt.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtshyhfapn.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtehfamoqr.html

C#:   class User {}
来源：http://hz.gogol.net.cn/gterwqzbaz.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtuawrrrcq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shangyingyoupin.top/gtfpstsuro.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gthlrplrbs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtcdpotwqx.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtxexzkzkx.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtpjkzdymw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtcswnmygw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxuanxn.top/gtoxefarei.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxinkj.top/gtybnbjdsn.html

[G03] 实例属性
来源：http://hz.xuanzx.com/gtvdeyiaxa.html

Py:   self.name = "x"
来源：http://hz.tanke756.top/gtjfjbehth.html

PHP:  public string $name = "x";
来源：http://hz.nwbrower.top/gtfiavpujn.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtppzmutyy.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtpmgnljuv.html

Java: private String name;
来源：http://hz.cheryme.top/gtzsibnndu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtexwehxwo.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtbwqnkqlw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtbvjpvrvc.html

[G04] 定义方法
来源：http://hz.nwbrower.top/gttwndtiga.html

Py:   def greet(self): return self.name
来源：http://hz.0kj1m.cn/gtuibydjja.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtiqrzmrel.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtrlqqyord.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtrjsdwqmw.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangtech.top/gteuaqqmxe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtucayxnml.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtjqzvtsiv.html

C#:   public string Greet() => Name;
来源：http://hz.hywenlv.cn/gtrqcnzujt.html

[G05] 继承
来源：http://hz.yj202588.top/gtvmqrolpx.html

Py:   class Admin(User): pass
来源：http://hz.xziqi.cn/gtfrjjgciu.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtsxnybfto.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtbxnudtij.html

TS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtqwflnnzw.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtbrqyccts.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtjhjhqdzb.html

Ruby: class Admin < User; end
来源：http://hz.smart0.xyz/gtaypdsnvg.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtetersixf.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtdjvfkprl.html

Py:   def greet(self): return "admin"
来源：http://hz.havefunace.top/gthmngvhmr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtbywfwobt.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtwexukhqy.html


<!-- 参考信息 -->