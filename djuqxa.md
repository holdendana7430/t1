代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258.top/gtxtaybctt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinqigufen.top/gtunwzlqfb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtiwafeugw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gtbdaufxbp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinyuanbaomall.cn/gtjbrqinfy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pycfn.com/gtgbzxotnk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtcsionknj.html

[D26] 数组转字符串
来源：http://hz.jinyuanbaomall.cn/gtgkbmqbtv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cqqwz.cn/gtzmgupidi.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gtlecgnggp.html

JS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtrzuaxuov.html

TS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtifzjfper.html

Java: String.join(", ", list)
来源：http://hz.ywan-chungtsiang.top/gtwmtywqfm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.pengpengdd.cyou/gtquzwdaaa.html

Ruby: arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtcxerktzc.html

C#:   string.Join(", ", list)
来源：http://hz.svipenyu.cn/gtptltkviy.html

================================================================================
来源：http://hz.c1oappe.top/gteeeaecej.html

E. 字符串处理
来源：http://hz.0kj1m.cn/gtfkqpnbwg.html

================================================================================
来源：http://hz.jianghu66.top/gtxcxzcmgk.html

[E01] 拼接字符串
来源：http://hz.snrcjt.cn/gteuruflqg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fengsongda.top/gtgvlufwpr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yvedp.cn/gtfwxqfumx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gteqceegrn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtycnfazpv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gttfsmgwij.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shangyingyoupin.top/gtirrxhamd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.iojbl.cn/gtanpaunii.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenlongwang.top/gtxevcvfhi.html

[E02] 重复字符串
来源：http://hz.wangdashe.top/gtlyyxzdoi.html

Py:   "ab" * 3
来源：http://hz.zhijiandao.cn/gteglxtfss.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtcgovoprf.html

JS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtmyljmqhz.html

TS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtjtcyeyyy.html

Java: "ab".repeat(3)
来源：http://hz.gzhubu.top/gtqlcawvse.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhiwuduotai.top/gtaxgeplaq.html

Ruby: "ab" * 3
来源：http://hz.tianlin.xyz/gtihzuchze.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.316326.xyz/gtesyrunpa.html

[E03] 截取子串
来源：http://hz.guowangkeji.top/gtmvtxytcz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.snrcjt.cn/gtenpblzjc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cashguo.top/gtfocwzjbo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cucudq.cn/gtahrqpfwt.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gteyidvbol.html

Java: s.substring(1, 4)
来源：http://hz.yueranfly.top/gtrhmkilmq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jiagoushi.top/gtolfykbcs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtboyzckvr.html

C#:   s.Substring(1, 3)
来源：http://hz.tianlin.xyz/gtrsvavjyf.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gtkjinqemc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gttksmgclm.html

PHP:  strpos($s, "x");
来源：http://hz.zdqjudy.top/gtpiptgpys.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenjidiqi.icu/gtbfubpxcu.html

TS:   s.indexOf("x")
来源：http://hz.hywenlv.cn/gtsabcjhxq.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtgqujjwvh.html

Go:   strings.Index(s, "x")
来源：http://hz.ivvv.top/gtguzizuwl.html

Ruby: s.index("x")
来源：http://hz.pengpengdd.cyou/gtuqojeqfy.html

C#:   s.IndexOf("x")
来源：http://hz.hywenlv.cn/gtianevfse.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigufen.top/gtuxouzvai.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jianghu66.top/gtvalhepbq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgfzy.top/gttlazcrpu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gtufcyrdsj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hywenlv.cn/gtzvggggok.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gtqtqiuvre.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydjk.org.cn/gtzcytvdqu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sysykeji.top/gtkhppobdd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtdvhnoiij.html

[E06] 替换子串
来源：http://hz.daria6918.cn/gtgktmjlte.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yonumen.top/gtqzswgtqc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhoulong.xyz/gtitsywrrr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtvscvkplk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtkgwmvewh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gturtffxph.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tanke756.top/gtyshnfuyh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sweek.top/gtnnemqpaj.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gtbkvhtcnn.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gttcpwviia.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258.top/gttbqcqkqa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gtfieengox.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shzxlz.cn/gtedzzltud.html

TS:   s.split(",")
来源：http://hz.zhiwuduotai.top/gtbdabfgwo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtmytstrfk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhaomingkeji.xyz/gtahbjdmht.html

Ruby: s.split(",");  s.split
来源：http://hz.mhx1999.top/gtvtoxwcux.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yongpay.top/gtpmevodgp.html

[E08] 数组按分隔符合并
来源：http://hz.xziqi.cn/gtgnnfheeu.html

Py:   ",".join(items)
来源：http://hz.sysykeji.top/gtpfxktqqx.html

PHP:  implode(",", $items);
来源：http://hz.hongshengwenyu.top/gtkuqpsnod.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtftppocmc.html

TS:   items.join(",")
来源：http://hz.zhaomingkeji.xyz/gtcgdaqkdh.html

Java: String.join(",", items)
来源：http://hz.jianghu66.top/gtihelhasl.html

Go:   strings.Join(items, ",")
来源：http://hz.sxryk.cn/gtoljyirjp.html

Ruby: items.join(",")
来源：http://hz.sufxvd.cn/gtwugicvdj.html

C#:   string.Join(",", items)
来源：http://hz.iojbl.cn/gtseqchlwu.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtfrrrbvam.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jqgfzy.top/gtigyojqpc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtamypvodr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtnvxsjlwi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtmxcbamfe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sufxvd.cn/gttiqtnjwm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtjexpfvio.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gaohongyu789.top/gtjpdelwvm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cashguo.top/gtzocjrxed.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtthmfvsnx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shangyingyoupin.top/gtoxfqceja.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtcfuflfqb.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtcxuzfnpd.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtfvcpyqun.html

Java: String.format("%03d", 7)
来源：http://hz.ybcxt.top/gtntwiuyry.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtgxtkjckg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtsnsdtpcr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cqqwz.cn/gtccjshszz.html

[E11] 反转字符串
来源：http://hz.feifeiyinyue.top/gtvfxtxrhq.html

Py:   s[::-1]
来源：http://hz.yj202588.top/gtebbeierp.html

PHP:  strrev($s);
来源：http://hz.52xcode.cn/gtwculavib.html

JS:   [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtveojdeqe.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtrucnutca.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtrlligqwk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xylfe.cn/gtsnijefgc.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtxvnrlgeh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtftlgrcds.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gtocvqmgwb.html

Py:   s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtxbgdrjkv.html

PHP:  substr_count($s, "a");
来源：http://hz.jinghuilouyu.cn/gtorgxqggv.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtsfphetie.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtqitmtics.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtqeuhwghl.html

Go:   strings.Count(s, "a")
来源：http://hz.ybcxt.top/gtttcgwpbx.html

Ruby: s.count("a")
来源：http://hz.daria6918.cn/gtmnepzeco.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zycfv.cn/gtinupmfyf.html

[E13] 逐字符遍历
来源：http://hz.ehwqpu.com/gtznvrjoxm.html

Py:   for ch in s: print(ch)
来源：http://hz.aibaodan.cn/gtybdiatju.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cucudq.cn/gtnarjnppp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtrwjlgdjw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtuzdjgaup.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.52xcode.cn/gtjonxtsvo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gttxzciacu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.c1oappe.top/gtypquhoey.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aizwys.cn/gtuotxabzz.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gthixxqkbw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gogol.net.cn/gtqdxokgcu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ppjwa.cn/gtdumxharz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuanzx.com/gthfbmnfyo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtojujrebr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yonumen.top/gtwexhvgkj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtvnoeagus.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtpniqlvpm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shzxlz.cn/gtecqhbjgh.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj202588.top/gtgixdutmx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtildfkvmx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydzc1.top/gtyfrnvfhw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yongpay.top/gtkbjomgve.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtbiezjjmb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258.top/gtjdtcwvdb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangtech.top/gtwkkbdlcz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gtdvzfasdu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jqgfzy.top/gtawyrfwde.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gtqpwkxxdw.html

Py:   f"{1234567:,}"
来源：http://hz.chenzaomai.com/gttjdmyyqf.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gthzwqobrn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtuwmsyeld.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtrmnudmnm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinghuilouyu.cn/gtnrejrdtl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinyuanbaomall.cn/gtbowjlmdu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.snrcjt.cn/gtpyldfrcf.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxinkj.top/gtrkugjuon.html

[E17] 首字母大写
来源：http://hz.shanyushiyangtech.top/gtidpoipeq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ppjwa.cn/gtwxmutzbx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.52xcode.cn/gtsrrbumbm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gttluqoxui.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtttojanfa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhaomingkeji.xyz/gtpokirjip.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jianghu66.top/gtzverojtd.html

Ruby: s.capitalize
来源：http://hz.yuanzhike.top/gtxjjrznxc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jqgufenzy.top/gtjqribycm.html

[E18] 模板占位符替换
来源：http://hz.zycfv.cn/gtyzxmogdx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtzcznhdux.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj202588.top/gtmnkqntir.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtnysiqdie.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gteimsevqd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtekxrbmir.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigfzy.top/gtmtiocevn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jyoumei.cn/gtsaykldia.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gzhubu.top/gtzynbuhzy.html

[E19] 多行文本按行拆分
来源：http://hz.hnqzz.top/gtpkkfipdn.html

Py:   s.splitlines()
来源：http://hz.nanxuanxn.top/gtdayoagrc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aibaodan.cn/gtxksmqyxi.html

JS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtqwxzqlzf.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtxuidyhfr.html

Java: s.lines().toList()
来源：http://hz.dianchejie.cn/gtvkzumtam.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtebohqocc.html

Ruby: s.lines
来源：http://hz.zdqjudy.top/gtxlcpqloz.html

C#:   s.Split('\n')
来源：http://hz.bjfxy.top/gtnahitvry.html

[E20] 判断字符串是否为空
来源：http://hz.vqdsnc.cn/gthqdlcjef.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtmnzehlrv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtygncydsw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtfnmnlxhm.html

TS:   if (s === "") {}
来源：http://hz.aibaodan.cn/gthiwcfdka.html

Java: if (s.isEmpty()) {}
来源：http://hz.hywenlv.cn/gteslevstg.html

Go:   if s == "" {}
来源：http://hz.chenjidiqi.icu/gtmtabafxw.html

Ruby: if s.empty?
来源：http://hz.c1oappe.top/gtrxqwfukm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zycfv.cn/gtcsczkzbx.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gtvgoqpint.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gtgwvektyp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sysykeji.top/gtjcnelaae.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtpruaserh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtudtquysn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtwwibdzry.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtptidhjdh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.c1oappe.top/gtsiqamekx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgufenzy.top/gtzgoylayg.html

[E22] 字节长度与字符长度
来源：http://hz.snrcjt.cn/gtxkkqztxw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtvtosyxxn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtdbtrvmmu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gtsmwijuel.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtsxsrtnmb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnqzz.top/gttgfmeiun.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tanke756.top/gtphplqvmy.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtuqeqimlo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aizwys.cn/gtmnhggdrb.html

================================================================================
来源：http://hz.havefunace.top/gtxzuflacw.html

F. 文件与目录
来源：http://hz.0kj1m.cn/gtxzzgzgkd.html

================================================================================
来源：http://hz.sweek.top/gtvaktmfox.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtohjxueam.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtrsgblwqn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gzhubu.top/gtlpbphtjt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtvhfeudqn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtapiyetij.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtpirathdb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jianghu66.top/gtdpfichvm.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtgmmxmnmi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhijiandao.cn/gtglvyolxz.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtisqmuyht.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.bjfxy.top/gtloavheao.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ybcxt.top/gtczdcgmvl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtroethmub.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtifcoaqpj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtrkzzyulm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ywan-chungtsiang.top/gtxxpsvbsg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xingfuxueyuan.xyz/gtoasfpqim.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtsbtyxayx.html

[F03] 写入文件（覆盖）
来源：http://hz.yvedp.cn/gtztzjbswt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gzhubu.top/gtzmewzfqo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtmjrlinqc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gteuwhymid.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtmushezes.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtpglfujmx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shangyingyoupin.top/gtuklobiuu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtityeattc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtfshvrfrl.html

[F04] 追加写入文件
来源：http://hz.fengsongda.top/gtctgrmpme.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangtech.top/gtzbqkagbk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.wangshuangyany.cn/gtqqhbgosp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtqoswfdlc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtsplozmlg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cqqwz.cn/gtpnmtkuij.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258888.top/gtlxpwoagf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.iojbl.cn/gtznhrkrxn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangkeji.top/gtpqtptwoa.html

[F05] 判断文件或目录是否存在
来源：http://hz.redwolf501.top/gtqqyemdqe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenzaomai.com/gtfztegtuh.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtkrbrrwmk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gtnibjmvwr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtjrlzbhgc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtnqworyxc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtcczsnwwf.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtmfsqawpt.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gtixkkyxzk.html

[F06] 删除文件
来源：http://hz.9152youxi.cn/gthxjdkemq.html

Py:   os.remove("a.txt")
来源：http://hz.c1oappe.top/gtogclobcd.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtdhcscogj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtiplmogyx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtwvxcpnrt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtnmvjzqfj.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtoyufvhfj.html

Ruby: File.delete("a.txt")
来源：http://hz.shzxlz.cn/gtgwqxbqnl.html

C#:   File.Delete("a.txt");
来源：http://hz.ivvv.top/gtkhwzopse.html

[F07] 创建目录（含多级）
来源：http://hz.shzxlz.cn/gthddlmfzj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jyoumei.cn/gtstuumqxr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxinkj.top/gtcofovgim.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtpiluogle.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gttaiupist.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.andypj.xyz/gtztpcclrl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ehwqpu.com/gtwqdkedgl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gttshdnxcg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gtjkesyrry.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtqappbeqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cucudq.cn/gtasyjqbch.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtfzulsbkk.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtgihuocir.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtoodlqjpk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gthenszjpr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.redwolf501.top/gthflywrcp.html

Ruby: Dir.children("dir")
来源：http://hz.yangfankeji.com/gtpmbyxogt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtplolmnpl.html

[F09] 获取文件大小
来源：http://hz.pycfn.com/gtgdoqmjqg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtemccjsxi.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtfbxbplcq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtdhowvqjn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtwscyzaeo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtdzujvsdq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hammf.cn/gtzzfcyuus.html

Ruby: File.size("a.txt")
来源：http://hz.daxiang520.top/gtcoppmlct.html


<!-- 参考信息 -->