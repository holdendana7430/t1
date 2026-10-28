代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gogol.net.cn/gtmqpsygvt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.smart0.xyz/gtjebgwovh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yongpay.top/gtdodlncki.html

[D26] 数组转字符串
来源：http://hz.yonumen.top/gtsqlkfoia.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hammf.cn/gtgtbmpnet.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtnhgspnqq.html

JS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtcqjayshu.html

TS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtiypohwtw.html

Java: String.join(", ", list)
来源：http://hz.sxryk.cn/gtuitfvsjz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtlrykfsim.html

Ruby: arr.join(", ")
来源：http://hz.jqgufenzy.top/gtmtzxwhou.html

C#:   string.Join(", ", list)
来源：http://hz.ybcxt.top/gtintutxlz.html

================================================================================
来源：http://hz.shzxlz.cn/gtdtwmxqpg.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtrsjftrya.html

================================================================================
来源：http://hz.fzhhl.top/gtkjegozuh.html

[E01] 拼接字符串
来源：http://hz.zhiwuduotai.top/gtpuffcmme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258888.top/gtghudpzca.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgufenzy.top/gtdsllrcsn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtactusail.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtdqfholtb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gogol.net.cn/gtsrtcoqoe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ydjk.org.cn/gtkbadtebl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtbmveyqrv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xziqi.cn/gtipreeeew.html

[E02] 重复字符串
来源：http://hz.vqdsnc.cn/gtewdkapsi.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtvumoznjm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtqfvewduw.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtpyqwxlys.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtotknjohv.html

Java: "ab".repeat(3)
来源：http://hz.hywenlv.cn/gttdzfwgkn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hywenlv.cn/gtbtrvsvxs.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gthwvxynqq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yueranfly.top/gtdmijwajm.html

[E03] 截取子串
来源：http://hz.xuanzx.com/gtrkjntxor.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gthsmakclo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigfzy.top/gtdevziyae.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxinkj.top/gtrlmzmtvu.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gtysnkuttk.html

Java: s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtlbwkaswo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtzjcnoips.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.iojbl.cn/gtmvnsgxmf.html

C#:   s.Substring(1, 3)
来源：http://hz.zhiwuduotai.top/gtbohzpbmb.html

[E04] 查找子串位置
来源：http://hz.feifeiyinyue.top/gtepaxvhuj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj20258888.top/gtdsptakpu.html

PHP:  strpos($s, "x");
来源：http://hz.ydjk.org.cn/gtpsvusyft.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.mhx1999.top/gthvzinlip.html

TS:   s.indexOf("x")
来源：http://hz.guannengcc.top/gtnjsfcqpt.html

Java: s.indexOf("x")
来源：http://hz.yongpay.top/gtdtnusmmo.html

Go:   strings.Index(s, "x")
来源：http://hz.gotoacloud.top/gtfjvphuiz.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtnjlmqwfz.html

C#:   s.IndexOf("x")
来源：http://hz.316326.xyz/gtklntprwn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guowangkeji.top/gtbsjjjvxs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj202588.top/gtwvjtzjmu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtipetnhjm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.havefunace.top/gtujbmzzfa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guannengcc.top/gtgxmfksyi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtypaebcqj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zdqjudy.top/gtymojwppk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhongyouzk.top/gthhuvzogm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.52xcode.cn/gtziaxczpa.html

[E06] 替换子串
来源：http://hz.hnxiangtu.top/gtjcpraype.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangshuangyany.cn/gtygyjzxsk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtwtsfypme.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtoqechimg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtdtqlpher.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtatxoxzzb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtkisznlba.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtmdvqqxks.html

C#:   s.Replace("a", "b")
来源：http://hz.shanyushiyangtech.top/gttrwplabt.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtxecbwhkn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pycfn.com/gtfnltaxfc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gtsxqlvopo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinqigufen.top/gtppgrhwtq.html

TS:   s.split(",")
来源：http://hz.wangdashe.top/gtbopeegrz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.0kj1m.cn/gtopytcoyc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydjk.org.cn/gtwzenamox.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtojdqroqc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinghuilouyu.cn/gtchtcklcf.html

[E08] 数组按分隔符合并
来源：http://hz.nanxinkj.top/gtvabjcsok.html

Py:   ",".join(items)
来源：http://hz.zdqjudy.top/gtcppjpzhx.html

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtpdecdwyy.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtdatrklfq.html

TS:   items.join(",")
来源：http://hz.zycfv.cn/gtoglserzr.html

Java: String.join(",", items)
来源：http://hz.zhijiandao.cn/gttrslvspo.html

Go:   strings.Join(items, ",")
来源：http://hz.sxryk.cn/gtcnkcsevc.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtmidwlckk.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtqxbfrzix.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtcpjexwoc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jlsjyb.cn/gtbccwoyle.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gtphecmwmb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gtogifkcxz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtuqapniej.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xylfe.cn/gtfgcdxhlh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pengpengdd.cyou/gtoreqbaqs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gogol.net.cn/gtctoxqbpx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.bjfxy.top/gtmhlkrxpk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.snrcjt.cn/gtjezfedlb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtpmqawvtd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gtbtaggpns.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gtujrmecwj.html

TS:   "7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtdjlxvuli.html

Java: String.format("%03d", 7)
来源：http://hz.yj202588.top/gttioonvlg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuanzx.com/gtzaekfgfj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gtvzbxizci.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.c1oappe.top/gtmtfqqnoq.html

[E11] 反转字符串
来源：http://hz.wangdashe.top/gteidmmhbk.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gthazzizjn.html

PHP:  strrev($s);
来源：http://hz.yonumen.top/gtbkgiswne.html

JS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtdhddobir.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtmttklfnj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtpkqebmrm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guowangkeji.top/gtgsbqgxav.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gtbjseudlo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtshtypodd.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtdwvjgjxz.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gtvfidcoqu.html

PHP:  substr_count($s, "a");
来源：http://hz.hnqzz.top/gtgtazieqo.html

JS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gtvxdhkmcr.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtkvozwhyp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtchvennov.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtrzeroqkl.html

Ruby: s.count("a")
来源：http://hz.yuxming.cn/gtmgaarfwz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258.top/gtaqydwgag.html

[E13] 逐字符遍历
来源：http://hz.shzxlz.cn/gtjbonapgs.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gtacsvmegr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gtaryzffzn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtcnjehpzu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtdblwuvjw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtsdwtkdfi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtjjlwujmw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cqqwz.cn/gthqkdluuh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.andypj.xyz/gtfofkptoe.html

[E14] URL 编码与 Base64
来源：http://hz.jyoumei.cn/gthclkkqaq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.snrcjt.cn/gtgvbqxacx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.mhx1999.top/gtmfqpiykv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.quarkkingdee.top/gtuqzcrmdw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pengpengdd.cyou/gtfulygyxe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtykirdiul.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jiagoushi.top/gtsmdxlppg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtxzikngek.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydzc1.top/gtmatrpujw.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtwtrjlfkp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cashguo.top/gtjjcwespx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangdashe.top/gtqghrpleg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sysykeji.top/gtrluwgzqf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hammf.cn/gtxboluhjh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ybcxt.top/gtqdyifkwn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tanke756.top/gtizrsawrp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jlsjyb.cn/gtqsgsdlmm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zdqjudy.top/gtngogypqg.html

[E16] 数字千分位
来源：http://hz.jyoumei.cn/gtxaisyhft.html

Py:   f"{1234567:,}"
来源：http://hz.9152youxi.cn/gtbkhyaqul.html

PHP:  number_format(1234567);
来源：http://hz.jqgfzy.top/gtjhjhddub.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtycrythsy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtcpnenpoa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtuzgojxka.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guowangkeji.top/gtsbdistvb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.vqdsnc.cn/gtddevzgtw.html

C#:   1234567.ToString("N0")
来源：http://hz.quarkkingdee.top/gtgnuandfc.html

[E17] 首字母大写
来源：http://hz.cqqwz.cn/gtbmjxcrvc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yvedp.cn/gtlvjtdgum.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zycfv.cn/gtyhlgdayz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gtovbghvhe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtynkrvveh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtcyuzacuu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gteflpdxeb.html

Ruby: s.capitalize
来源：http://hz.hammf.cn/gtykxhdgpz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtmofmjbze.html

[E18] 模板占位符替换
来源：http://hz.hnxiangtu.top/gtqeeadxjd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ehwqpu.com/gtokooyeco.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nwbrower.top/gtxotbaryi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtslbiwhth.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtxhlixhkx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtoujpxkvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.316326.xyz/gtngiewcjy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aibaodan.cn/gtwbqjnfho.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuanzx.com/gtskpiwgat.html

[E19] 多行文本按行拆分
来源：http://hz.shangyingyoupin.top/gtlfuvctcb.html

Py:   s.splitlines()
来源：http://hz.ybcxt.top/gtxlyfzolp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zycfv.cn/gttuptwnbc.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtialkxeip.html

TS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtqwrrypdr.html

Java: s.lines().toList()
来源：http://hz.yj202588.top/gttrabcxgn.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhoulong.xyz/gtylgjhocm.html

Ruby: s.lines
来源：http://hz.gotoacloud.top/gtbuhdanpq.html

C#:   s.Split('\n')
来源：http://hz.birdmap.top/gtjfrxtmrx.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtsukqgoke.html

Py:   if not s:
来源：http://hz.chenjidiqi.icu/gtubbrxpvv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.smart0.xyz/gtbdqvgvnd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xziqi.cn/gtbefgncgy.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gtocurcbbi.html

Java: if (s.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gtaqwifddm.html

Go:   if s == "" {}
来源：http://hz.0kj1m.cn/gtlsgswtxs.html

Ruby: if s.empty?
来源：http://hz.xylfe.cn/gtqzmempvt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtelgljfbh.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtbljyifud.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gtfgeydesi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigfzy.top/gtefbabegg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtwjsivitf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtckqcyqbp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtskfoktzy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtstjmvyyx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtqrpmtpwp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cheryme.top/gtkmujsrjx.html

[E22] 字节长度与字符长度
来源：http://hz.zhoulong.xyz/gtqybxqhne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yangfankeji.com/gtmqsvimbg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtaygyexmh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtgfpllrhl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtbnquzmje.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yonumen.top/gtdkvekflx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hammf.cn/gtmujgqjkv.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gtxqzlrwpq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtvfmaipgx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvrfzhxxk.html

F. 文件与目录
来源：http://hz.kuanghao11.cn/gtwhxqyjbp.html

================================================================================
来源：http://hz.hnqzz.top/gticaubgfe.html

[F01] 读取整个文件
来源：http://hz.yvedp.cn/gtnrymqewp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydjk.org.cn/gtrgmuddig.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yanxiufei.cn/gtfgcltine.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxinkj.top/gtuwfdoofu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jiagoushi.top/gttikshpji.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtlfsoswjl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtzsaiefsy.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gtizrwrdhj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gtunvqmiwb.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtdfrihvsl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gogol.net.cn/gtsaxagwjv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhongyouzk.top/gtkfzjkbre.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtdgepdibd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtyxpbwobf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtefthumii.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangkeji.top/gtbaaomvfc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gtcndchdck.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aibaodan.cn/gttlwaxepg.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gtwrpadsbo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.birdmap.top/gtrtgkgzdw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtadhwchjn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtpqjakkpj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtdeiwjflc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxinkj.top/gtlwvzstoo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.redwolf501.top/gtfqjwloen.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtrzuiyuhz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtyrfdfzoo.html

[F04] 追加写入文件
来源：http://hz.guannengcc.top/gtlcakhvcb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.redwolf501.top/gtmalcdqke.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yongpay.top/gtlgqpahfd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.havefunace.top/gtzvvwptts.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtzjrzfjxl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zycfv.cn/gthnaepwrt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.quarkkingdee.top/gtioenqnak.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnxiangtu.top/gtoddfnuqz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gtqlpwwroz.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtezdtutcu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangdashe.top/gtbjvtpjwv.html

PHP:  file_exists("a.txt");
来源：http://hz.gzhubu.top/gtgpgjnspc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gthabkyaiz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtzofnqufz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtcbfckufx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yanxiufei.cn/gtwxzkrozz.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigufen.top/gtcyrgpuwo.html

C#:   File.Exists("a.txt")
来源：http://hz.snrcjt.cn/gtismuixyd.html

[F06] 删除文件
来源：http://hz.aizwys.cn/gthrpwttvx.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtiohjohbc.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtqwtiglca.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtvsqimxvc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtoxrladys.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtoimsmcvq.html

Go:   os.Remove("a.txt")
来源：http://hz.cucudq.cn/gtkshpbdhu.html

Ruby: File.delete("a.txt")
来源：http://hz.birdmap.top/gtrvycoiao.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtyrshljol.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gthvaqctlw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuanzx.com/gtetvrjbdd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtgaixdmuz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtduehkwdr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtipgflumr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xinyue.icu/gttmsdifyn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtvyffduaf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cucudq.cn/gtyszuzbfs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gtufpytzip.html

[F08] 遍历目录
来源：http://hz.kuanghao11.cn/gtabbiuflw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gthwbaeipk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sysykeji.top/gtchqucwbf.html

JS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtvjrowxgf.html

TS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtppdgyquf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gtiwplpmyw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtgzqczvqt.html

Ruby: Dir.children("dir")
来源：http://hz.yvedp.cn/gtwvklviqf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.mhx1999.top/gtckpphhoa.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtmtndotai.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtbkafkfms.html

PHP:  filesize("a.txt");
来源：http://hz.xinyue.icu/gtgjolqmiy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtnujtoltt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtdsxmxczf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtlldlwmri.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gtxviydvtm.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gtjqdmlhuu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zycfv.cn/gtnneooskw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhongyouzk.top/gtnkxjtlrh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtkslhvopb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydzc1.top/gtopbwaixp.html


<!-- 参考信息 -->