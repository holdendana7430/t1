代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtoeofzgnz.html

TS:   s.slice(1, 4)
来源：http://hz.cqqwz.cn/gtdfdxninv.html

Java: s.substring(1, 4)
来源：http://hz.andypj.xyz/gtucmfllce.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gtjsyzgdib.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.fengsongda.top/gtymtnmusq.html

C#:   s.Substring(1, 3)
来源：http://hz.andypj.xyz/gtqzraeiqh.html

[E04] 查找子串位置
来源：http://hz.hnqzz.top/gtuacsfxsg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtwunrvgrj.html

PHP:  strpos($s, "x");
来源：http://hz.hammf.cn/gttcqegqio.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtexpmbqlq.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtlzxesems.html

Java: s.indexOf("x")
来源：http://hz.52xcode.cn/gtzhrjuvkq.html

Go:   strings.Index(s, "x")
来源：http://hz.hywenlv.cn/gtauhngozl.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtwmhndfmh.html

C#:   s.IndexOf("x")
来源：http://hz.jlsjyb.cn/gteatnycuy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ywan-chungtsiang.top/gtglcorupg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fzhhl.top/gtossxbpvp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yvedp.cn/gttxtdlgmw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtmlhddeip.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtsfgphzxi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtptukasbw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.316326.xyz/gtpiyazdcq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.9152youxi.cn/gtfuvmfthu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gaohongyu789.top/gtprmjmqmh.html

[E06] 替换子串
来源：http://hz.sysykeji.top/gtsibxevda.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtbhxrdhtc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gzhubu.top/gtjwtpnbbg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gttinbfyao.html

TS:   s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtaeppixam.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtsiyfyugn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtugfzcdes.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hammf.cn/gtohonedwn.html

C#:   s.Replace("a", "b")
来源：http://hz.fengsongda.top/gtqmwfixdp.html

[E07] 按分隔符拆分
来源：http://hz.tanke756.top/gtwoqjfijc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hywenlv.cn/gtlmfmvrhm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gotoacloud.top/gtiucvpbun.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zycfv.cn/gtnzroiuwv.html

TS:   s.split(",")
来源：http://hz.yongpay.top/gtgfsqpqkg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.dianchejie.cn/gtpjzptfvc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sweek.top/gtwwehzriw.html

Ruby: s.split(",");  s.split
来源：http://hz.zhijiandao.cn/gtlyyrgmje.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.haohaochexian.top/gttxclimjd.html

[E08] 数组按分隔符合并
来源：http://hz.ywan-chungtsiang.top/gttdgtazpp.html

Py:   ",".join(items)
来源：http://hz.sysykeji.top/gtwcqnzaey.html

PHP:  implode(",", $items);
来源：http://hz.ybcxt.top/gtyeaxaqrj.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtcbntkzpw.html

TS:   items.join(",")
来源：http://hz.hysaishi.cn/gtnvxwrhzy.html

Java: String.join(",", items)
来源：http://hz.sufxvd.cn/gtmurghjct.html

Go:   strings.Join(items, ",")
来源：http://hz.hammf.cn/gtamxahvec.html

Ruby: items.join(",")
来源：http://hz.jlsjyb.cn/gtykhryhwt.html

C#:   string.Join(",", items)
来源：http://hz.yongpay.top/gtucebkhfo.html

[E09] 去除所有空白字符
来源：http://hz.zhongyouzk.top/gtuapiywvz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtacakcxgd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxuanxn.top/gtoarpxuhh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtyumvjqub.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtoxxkmprc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtnwjuckqs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtreykjtnb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.0kj1m.cn/gtloqqmmtx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtvlezdzyu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydjk.org.cn/gtoiyulppy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtculukkag.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gthsgwswfg.html

JS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gtoanajjit.html

TS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtgccabzes.html

Java: String.format("%03d", 7)
来源：http://hz.redwolf501.top/gtbhjqzjqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtmsrewjnw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtwpjzvjnt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtwsrdiwrn.html

[E11] 反转字符串
来源：http://hz.cqqwz.cn/gtwryipyir.html

Py:   s[::-1]
来源：http://hz.havefunace.top/gtqhspfpki.html

PHP:  strrev($s);
来源：http://hz.fengsongda.top/gtbcmhcjkj.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gthjggdijd.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtvdwczncs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhengqikj.top/gtdzrsypra.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtbeplzhxs.html

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtanzatrks.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtkmvvkbiu.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gthfvxcqko.html

Py:   s.count("a")
来源：http://hz.quarkkingdee.top/gtihmdckyn.html

PHP:  substr_count($s, "a");
来源：http://hz.c1oappe.top/gtjnjxnqyj.html

JS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtbqvbdnbs.html

TS:   s.split("a").length - 1
来源：http://hz.zhongyouzk.top/gttigeivng.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xziqi.cn/gtfhwennha.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtatyoixuh.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gtbliigkcp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhijiandao.cn/gtbtmtbkjy.html

[E13] 逐字符遍历
来源：http://hz.cucudq.cn/gtbbraluzi.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtbfgbfkli.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gtfphksttc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gtjgtnzykt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtowhscttf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtdthdvcla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.svipenyu.cn/gtpoaytjbr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhiwuduotai.top/gtizknmsub.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxinkj.top/gthnmngqor.html

[E14] URL 编码与 Base64
来源：http://hz.chenlongwang.top/gtvbxuwqqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yvedp.cn/gtlvcrwnhx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj202588.top/gtqivqllqj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tanke756.top/gtvstokuvm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gtgvkkwcjs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnqzz.top/gteeyxwruv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.smart0.xyz/gtgzcguate.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtkebavwar.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtpbbrqzio.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gtkiepvpze.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dianchejie.cn/gtlujzhkys.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ppjwa.cn/gtgqnfboci.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gticqlgurv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.0kj1m.cn/gtzhgtslnp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gtqxsgxyew.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yangfankeji.com/gtfpkmovxe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.quarkkingdee.top/gtcevqlixh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cheryme.top/gtjscbjysy.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gtcgxpnabj.html

Py:   f"{1234567:,}"
来源：http://hz.quarkkingdee.top/gtdtoclfss.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtdcmgykoh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtxswvobuq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtcmyyvpcp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gaohongyu789.top/gtxunnojfn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtknttjkmj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtdbywjtzb.html

C#:   1234567.ToString("N0")
来源：http://hz.xinyue.icu/gtjlsuqawk.html

[E17] 首字母大写
来源：http://hz.jinyuanbaomall.cn/gteejqdllb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.52xcode.cn/gtnfnpbokp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shuidangran.top/gtugalfonp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtmwynqasi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtzkovkckt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.vqdsnc.cn/gtonnljmha.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangdashe.top/gtvrwgnxty.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtqmmvogsd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hnqzz.top/gtoxpqoisc.html

[E18] 模板占位符替换
来源：http://hz.xuanzx.com/gtbzjdovbv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cashguo.top/gtkinwoakd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ehwqpu.com/gtnbhoqajb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtfcloiyqm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtvxohjjwa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtqjghjysm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.meibo888.top/gtsevrijfz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhongyouzk.top/gteuzcqtte.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shuidangran.top/gtrjucosfg.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtroejvfrn.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gtqnacvliy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtaalijhsl.html

JS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtufneoojt.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtkutitgjn.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtqrdgfokj.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtfdvebpkl.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtntiaivei.html

C#:   s.Split('\n')
来源：http://hz.pycfn.com/gtugrixxre.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gthyvewajc.html

Py:   if not s:
来源：http://hz.wangshuangyany.cn/gtwpvgtvsi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xziqi.cn/gtmvpvgwvn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aizwys.cn/gtigadfxhb.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtdypebrgk.html

Java: if (s.isEmpty()) {}
来源：http://hz.sweek.top/gtuptrwdub.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtmltxvrbf.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtgghnfltn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhixingplan.top/gtfcjoighw.html

[E21] 超长截断加省略号
来源：http://hz.tanke756.top/gtcyqollzw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtbfvpbfvu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtcixnjlpt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtfqktqfvp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtabtdzibd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtwmrbrtkc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ybcxt.top/gtmblqggwn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhongyouzk.top/gtpywzwkxm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gtrtchuwoi.html

[E22] 字节长度与字符长度
来源：http://hz.shzxlz.cn/gtimlcdlba.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtegabnskn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtgnsyczgy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhijiandao.cn/gtqrageebk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtfzflhngl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daxiang520.top/gtwztrhndl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daria6918.cn/gtsipakzva.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gtmbudcyix.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gtydcfptcv.html

================================================================================
来源：http://hz.cqqwz.cn/gtwtsqppqn.html

F. 文件与目录
来源：http://hz.316326.xyz/gtscusrivk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmdmrioxg.html

[F01] 读取整个文件
来源：http://hz.gaohongyu789.top/gtfsucrcbd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtvnkhyxla.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtmrmkpgyn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhaomingkeji.xyz/gtytturgwv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtsgusmsqq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtnpvjtafz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgufenzy.top/gtdwdelpnu.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtxotizsnz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtuvdbdmia.html

[F02] 逐行读取文件
来源：http://hz.cqqwz.cn/gtnpucqisv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gzhubu.top/gtvkfktzdm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtwolpsgqa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.feifeiyinyue.top/gtjroutqww.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtgbeurays.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtqgsahcok.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cucudq.cn/gtnjsfzqyz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xingfuxueyuan.xyz/gtuebyvxhg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinghuilouyu.cn/gthkbmxmrd.html

[F03] 写入文件（覆盖）
来源：http://hz.dashuyun.cn/gtcawjhzon.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xinyue.icu/gtnzfivqps.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnqzz.top/gtyxfqibwm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gthqwpjrwe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtrctrdhci.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.haohaochexian.top/gtcpiewygc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtpyywkmgk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shzxlz.cn/gtxrcetdgt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yueranfly.top/gtwjybzgyo.html

[F04] 追加写入文件
来源：http://hz.guannengcc.top/gtopbcihwk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtnxhrqofx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.wangdashe.top/gtnwhnizbt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.52xcode.cn/gtqxxvvmtw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtfqmkxqza.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ehwqpu.com/gtutyzpptn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtmghwhxsc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtkheymmqo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangtech.top/gtqhzzqrcd.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtasvsaaxs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtfiqnrkbs.html

PHP:  file_exists("a.txt");
来源：http://hz.aibaodan.cn/gtukikquyp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gthdamezqz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtbqgogzjj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtggicdaqq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cashguo.top/gtouzemrjg.html

Ruby: File.exist?("a.txt")
来源：http://hz.daria6918.cn/gtjaftvfzf.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtkdwcpqne.html

[F06] 删除文件
来源：http://hz.guowangkeji.top/gttptzxipk.html

Py:   os.remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtsohxudwy.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtzznmqolz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtgbkamglq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtutcvungr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtphduilhd.html

Go:   os.Remove("a.txt")
来源：http://hz.ehwqpu.com/gteabubstv.html

Ruby: File.delete("a.txt")
来源：http://hz.hfpthk.cn/gttilgxgfx.html

C#:   File.Delete("a.txt");
来源：http://hz.ydzc1.top/gtuxwfmvhs.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtrdhmfksu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigfzy.top/gtzhvsvrsb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtsdvxjrvy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtceupenlg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtupzbhptt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtyfvznejz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtupuohjhl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gthmwxxeys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.kuanghao11.cn/gtjimyopbq.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtmgesslfe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yanxiufei.cn/gtfqgshlhi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.havefunace.top/gtzbuicqxx.html

JS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtngmxtgmt.html

TS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gthvjnvrdy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtqfcqhenp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtzroyjeyk.html

Ruby: Dir.children("dir")
来源：http://hz.yj202588.top/gtueycoshh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tanke756.top/gtjbocnect.html

[F09] 获取文件大小
来源：http://hz.wangshuangyany.cn/gthwcgsvpm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gtgzosgjjl.html

PHP:  filesize("a.txt");
来源：http://hz.xziqi.cn/gttmnxohoe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtmthudygh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtimiiywkb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtdizamnqv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.birdmap.top/gtfrojfayp.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtcchfblip.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gthptltmso.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gteezjugjw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtdkaexrca.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gthoyibagg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtlphelnfc.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gtvlychaxe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtmwbwhity.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yangfankeji.com/gtblvgdddz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gthprtqhhd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtlnljnydy.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtqknxnixe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gttbcpvrfb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jlsjyb.cn/gtxdrzwdal.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtjvxwqffg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtfhrvzwcv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nwbrower.top/gtaabbqpcp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtesrcterj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtitekjdpo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.c1oappe.top/gtqeswpedp.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtnbhcmdxt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daxiang520.top/gtjobtyzdu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gtntdtiamx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhongyouzk.top/gthtgkrozv.html

TS:   // 同上
来源：http://hz.mhx1999.top/gtdgajhuaf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nwbrower.top/gtfphrfmtl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhongyouzk.top/gtyogajwgy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zycfv.cn/gtuksrnhli.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtkpiatsfa.html

================================================================================
来源：http://hz.xziqi.cn/gtjctxxkwp.html

G. 面向对象
来源：http://hz.sysykeji.top/gtzkdsotkm.html

================================================================================
来源：http://hz.0kj1m.cn/gtixknbfos.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtrrruwfvi.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gtnrfrbnum.html

PHP:  class User {}
来源：http://hz.hongshengwenyu.top/gtfeiywyxh.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtpfaasyrk.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtqzrlugcs.html

Java: class User {}
来源：http://hz.tanke756.top/gtqyzrggju.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtvtdrinls.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtyerzaarp.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtwewlsorl.html


<!-- 参考信息 -->