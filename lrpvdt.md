代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.52xcode.cn/gtstqvhsmo.html

JS:   items.join(",")
来源：http://hz.gaohongyu789.top/gtcakfbsob.html

TS:   items.join(",")
来源：http://hz.nwbrower.top/gtnjqdfzyi.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gteyqipcwy.html

Go:   strings.Join(items, ",")
来源：http://hz.gogol.net.cn/gtbfyvisio.html

Ruby: items.join(",")
来源：http://hz.tanke756.top/gtbzesdxje.html

C#:   string.Join(",", items)
来源：http://hz.ppjwa.cn/gtplzxajqp.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gtptqloctx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.bjfxy.top/gtasfyaxup.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gzhubu.top/gthqfrfehx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtrzzzmcnu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gtrewjojrm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.haohaochexian.top/gtfkdvvyxx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jyoumei.cn/gtqbxrimew.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtchhvbqhw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhoulong.xyz/gtxiffqmeo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tanke756.top/gtaylybcxw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhoulong.xyz/gtszgqrmvs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hfpthk.cn/gtqaqiddqc.html

JS:   "7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtzxgeging.html

TS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtonwrchpk.html

Java: String.format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtpxybvbuu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtinkjvdmj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tanke756.top/gtxilnsenx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.iojbl.cn/gthcdxthok.html

[E11] 反转字符串
来源：http://hz.pycfn.com/gtmxqvgkdn.html

Py:   s[::-1]
来源：http://hz.316326.xyz/gtwsgaaife.html

PHP:  strrev($s);
来源：http://hz.zhijiandao.cn/gtpbvpmszv.html

JS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtplkchpic.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtldxzjmtg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yangfankeji.com/gtmlznedmj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hysaishi.cn/gtjnkcvzja.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gtfvhtkbch.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtlzoyuujv.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtdcbppuyc.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gttodrzbvr.html

PHP:  substr_count($s, "a");
来源：http://hz.jiagoushi.top/gtcbmsruhh.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtxozijqkn.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangkeji.top/gtpsipcxek.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtxyhfxdup.html

Go:   strings.Count(s, "a")
来源：http://hz.hnqzz.top/gtcfydqmoe.html

Ruby: s.count("a")
来源：http://hz.iojbl.cn/gtdtzzjtfe.html

C#:   s.Count(c => c == 'a')
来源：http://hz.quarkkingdee.top/gtqslxaqur.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtawwtpube.html

Py:   for ch in s: print(ch)
来源：http://hz.gzhubu.top/gtkkafxjep.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daxiang520.top/gtvqsowiyp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtrqcflsau.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtveuirwep.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nwbrower.top/gtxcfruohx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aizwys.cn/gtmggsbtda.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtxcipzdtf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pycfn.com/gtjwnuudgt.html

[E14] URL 编码与 Base64
来源：http://hz.pengpengdd.cyou/gtxwjgthms.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gtrssxasue.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgufenzy.top/gtspxnpvlr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dashuyun.cn/gtvoylufwm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtaqmtaijk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhijiandao.cn/gtkqejtuxg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtsdrbsfvd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tianlin.xyz/gthwvzfjso.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.52xcode.cn/gtpnrevrzw.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtkpsnoaxv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gtqqkbczsk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuanzhike.top/gtyexrgyyt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gtzplipzsu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtdicvwfty.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuanzx.com/gtnqxanxvk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtkofyssjx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtjcihvcsx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gtjosllhhg.html

[E16] 数字千分位
来源：http://hz.hnxiangtu.top/gtldgdmzcw.html

Py:   f"{1234567:,}"
来源：http://hz.meibo888.top/gtotmvrqms.html

PHP:  number_format(1234567);
来源：http://hz.yvedp.cn/gtjucxoagg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtlhktjdrk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtvtjgbokd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nwbrower.top/gtywcgoids.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtkwrcungw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yueranfly.top/gtcrlnxvmy.html

C#:   1234567.ToString("N0")
来源：http://hz.sxryk.cn/gtofrwscdg.html

[E17] 首字母大写
来源：http://hz.9152youxi.cn/gtvdrfgzjc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gttcwboqcg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtnvtjwwvf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtcjiujidt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtmknpuawv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guowangkeji.top/gtkliqcfdg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhongyouzk.top/gtmuxcuwjx.html

Ruby: s.capitalize
来源：http://hz.ehwqpu.com/gtymmygwkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gtdkrlreps.html

[E18] 模板占位符替换
来源：http://hz.redwolf501.top/gtgelzsqqw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtidlsdjet.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxuanxn.top/gtzvdmhnsx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtklcamfgr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtwpdtavlu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.vqdsnc.cn/gtfqoearyu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxuanxn.top/gtwjmvqnys.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gogol.net.cn/gtcvuhijag.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangshuangyany.cn/gtjayjlcqo.html

[E19] 多行文本按行拆分
来源：http://hz.yongpay.top/gtuoipiieg.html

Py:   s.splitlines()
来源：http://hz.zhaomingkeji.xyz/gtvzvupsuj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtayqmrtja.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gtpfxcuuna.html

TS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtkjzesklf.html

Java: s.lines().toList()
来源：http://hz.ybcxt.top/gtdbegttif.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgufenzy.top/gtaebkckpr.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtdmikznmd.html

C#:   s.Split('\n')
来源：http://hz.xinyue.icu/gtdgbzcjat.html

[E20] 判断字符串是否为空
来源：http://hz.nanxuanxn.top/gtjsppkmeu.html

Py:   if not s:
来源：http://hz.bjfxy.top/gtjpfrjqzl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sweek.top/gturvxcjdd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtobqklrjv.html

TS:   if (s === "") {}
来源：http://hz.yuanzhike.top/gtfaqmvdrx.html

Java: if (s.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtqwzueeib.html

Go:   if s == "" {}
来源：http://hz.zhaomingkeji.xyz/gtenajpnif.html

Ruby: if s.empty?
来源：http://hz.hnxiangtu.top/gtymlzjufw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtlxixddgf.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtzgonwfpk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj202588.top/gtrqvkirfy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtqpxrwold.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtelmyezup.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtdaosmnfd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtkhjobndl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pycfn.com/gtyhylybsp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shzxlz.cn/gtlkzqpstc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtswzqmevv.html

[E22] 字节长度与字符长度
来源：http://hz.cdnleiting.top/gtlljiohjc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gtztxbupej.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhixingplan.top/gtqgbcjnxg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtecrtzrjm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtlyaddhrt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ybcxt.top/gtzdetbgdy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.kuanghao11.cn/gtjuxzabve.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtftjxshdu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtmkwrequm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthuqocmte.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gtqelaqull.html

================================================================================
来源：http://hz.cucudq.cn/gtixdmufgu.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtzzchvbbc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shanyushiyangkeji.top/gtfknibhza.html

PHP:  file_get_contents("a.txt");
来源：http://hz.mhx1999.top/gtqsliwhzr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dianchejie.cn/gtjdizlhtq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hammf.cn/gtzsgyzgpl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtwetzzspv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinghuilouyu.cn/gtewsachbu.html

Ruby: File.read("a.txt")
来源：http://hz.fengsongda.top/gtovrepvzs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sufxvd.cn/gtftsimftu.html

[F02] 逐行读取文件
来源：http://hz.tian-w.cn/gtdggcykfs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.quarkkingdee.top/gtvnoumwrz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtvetnltkl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtpwndcfhe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtackqbgvb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtzffgmapi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtcjamgqmf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhijiandao.cn/gtpliweaew.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gthkmostpn.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtapqsldli.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yongpay.top/gtrosjtckf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtgicglktb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtipdgrbxv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.meibo888.top/gtzkisefry.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtpivgnkqn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shzxlz.cn/gtoiewgjsb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.316326.xyz/gtoyjlogyc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xylfe.cn/gtbuukuzpg.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtmvqejoak.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gtgmevobek.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.quarkkingdee.top/gttlshmyyn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtrvokpvpg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtjfamfvwj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenzaomai.com/gtxfxcotch.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtaqtibwcx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yanxiufei.cn/gtjuzknpjb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtaowapisu.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gtdiorfevu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhaomingkeji.xyz/gtciiatbxz.html

PHP:  file_exists("a.txt");
来源：http://hz.jinghuilouyu.cn/gtpugtcrpw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gttmarjczc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtyoewauog.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtctovzawb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guowangkeji.top/gtqymjdmti.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtcmuonbqn.html

C#:   File.Exists("a.txt")
来源：http://hz.vqdsnc.cn/gtpxolmugj.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gtyfeiygzq.html

Py:   os.remove("a.txt")
来源：http://hz.fengsongda.top/gtacitbrba.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gtfxqzgeuy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gtvqtfrfnj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtgwtfjwwv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtwfosmwzx.html

Go:   os.Remove("a.txt")
来源：http://hz.sufxvd.cn/gtsvxligau.html

Ruby: File.delete("a.txt")
来源：http://hz.bjfxy.top/gtwrfffnvn.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gtllelrbbw.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtxlsuaomq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gaohongyu789.top/gtxiesooud.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtignqzgau.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gthdwjkjrk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtiszdhufp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenzaomai.com/gtetsssweh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yueranfly.top/gtejxabynx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.haohaochexian.top/gtyamounnt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtswimafgv.html

[F08] 遍历目录
来源：http://hz.hammf.cn/gtgrieswsq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gtbxphubxk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gtfqrqapyn.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtdrazhfan.html

TS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtioicmhlt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtrwgormab.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gtclnsfnti.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtcflovrrk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtvxsfqblb.html

[F09] 获取文件大小
来源：http://hz.hongshengwenyu.top/gtmkmrasts.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gthzvmlxse.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtgdwdfqnp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtfpcvxjgk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtutqcahqk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtnkcslvap.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ybcxt.top/gtmenzoqro.html

Ruby: File.size("a.txt")
来源：http://hz.tian-w.cn/gtckxeommj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daxiang520.top/gtqkbxpbmh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtzlxntbbd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtrnvadida.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigfzy.top/gtecjbjype.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtnewxrsws.html

TS:   path.extname("a.txt")
来源：http://hz.daxiang520.top/gtmnloxzwa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtobubdkkl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sysykeji.top/gtjjjcjnfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtdcwkzquz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gtiuetdpkk.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtrndlrrae.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtjemnbyli.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtsauiselo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtdacfywkq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gthjfdsbhw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuanzx.com/gtpkpeykjb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtihdjtvun.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtswgtaizv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtshxpqggi.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtenjjcgiy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.bjfxy.top/gtqugmgvwd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dianchejie.cn/gtknnoaflc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtcsxnxora.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtziumksyh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gtkeuesjjw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj202588.top/gtvmosaxbc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtzswqfxob.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dianchejie.cn/gtykbonxhy.html

================================================================================
来源：http://hz.ivvv.top/gtjgzadzis.html

G. 面向对象
来源：http://hz.daxiang520.top/gtljzhkrub.html

================================================================================
来源：http://hz.aizwys.cn/gtruxodktg.html

[G01] 定义类
来源：http://hz.zhongyouzk.top/gtsquuuvib.html

Py:   class User: pass
来源：http://hz.shuidangran.top/gtmpxewbwh.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gttqufsbbh.html

JS:   class User {}
来源：http://hz.feifeiyinyue.top/gtgdhaqrwj.html

TS:   class User { name: string = ""; }
来源：http://hz.ydjk.org.cn/gtdbgbomwc.html

Java: class User {}
来源：http://hz.ywan-chungtsiang.top/gtnfyctqmm.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtyqnteepy.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtytibfcyj.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtogztpwgz.html

[G02] 构造函数
来源：http://hz.zhongyouzk.top/gtjhidzgit.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtagdpplxg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtxmbyizmm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtuiuyxubg.html

TS:   constructor(public name: string) {}
来源：http://hz.hysaishi.cn/gtfjvyvrlp.html

Java: User(String name) { this.name = name; }
来源：http://hz.yvedp.cn/gtmkrnejok.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtdvwllziw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gttqxmeggl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yongpay.top/gtkaepmflh.html

[G03] 实例属性
来源：http://hz.gzhubu.top/gtglhqvcvs.html

Py:   self.name = "x"
来源：http://hz.mhx1999.top/gtlkwfjise.html

PHP:  public string $name = "x";
来源：http://hz.tian-w.cn/gtaelvbcza.html

JS:   this.name = "x";
来源：http://hz.yvedp.cn/gtwawvqllp.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gttyfkhkpn.html

Java: private String name;
来源：http://hz.sysykeji.top/gtczttepin.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtesxorefy.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtvidgprui.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zycfv.cn/gtdllsboku.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtpyfxdvto.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtkohqojck.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtwdjbsmle.html

JS:   greet() { return this.name; }
来源：http://hz.shuidangran.top/gtsgjagwzk.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtronxwlgw.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gtarhufcnv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtswpqusar.html

Ruby: def greet; @name; end
来源：http://hz.redwolf501.top/gtpuykrlwj.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtqbcslzkx.html

[G05] 继承
来源：http://hz.andypj.xyz/gtopobkjjc.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtqrpmjuei.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtnnhajkvl.html

JS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtroulkeax.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtzrfexole.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtjstzgpxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtgsszoslm.html

Ruby: class Admin < User; end
来源：http://hz.shzxlz.cn/gtblgvobpf.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtpanquavi.html

[G06] 重写方法
来源：http://hz.sweek.top/gtpgovmggj.html

Py:   def greet(self): return "admin"
来源：http://hz.ydzc1.top/gtlouyyebh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtgsiiqocg.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtysgqvngv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtbeumnfbs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtvlsjupom.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenzaomai.com/gtdpdpsbmw.html

Ruby: def greet; "admin"; end
来源：http://hz.zhengqikj.top/gtiwcoqyum.html


<!-- 参考信息 -->