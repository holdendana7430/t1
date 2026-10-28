代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.9152youxi.cn/gtplosgvmt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yongpay.top/gtxmroawye.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gtfukauumj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtrtowbwjj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.9152youxi.cn/gtvmjpboxt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.kuanghao11.cn/gtqnypyydh.html

[D25] Set 集合去重与交并差
来源：http://hz.jyoumei.cn/gtltcrcpgy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.meibo888.top/gtxarthuih.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ehwqpu.com/gtqybnstoq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yongpay.top/gtbvnhhylf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gterwjndjy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dianchejie.cn/gtekmhijps.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gttrblcavt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hfpthk.cn/gtyamlewin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangdashe.top/gtiwsfastj.html

[D26] 数组转字符串
来源：http://hz.hammf.cn/gtrtxsbiap.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jianghu66.top/gtzyfjgckq.html

PHP:  implode(", ", $arr);
来源：http://hz.cucudq.cn/gtuputcbuc.html

JS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtymtobgmj.html

TS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gttetmithi.html

Java: String.join(", ", list)
来源：http://hz.nanxinkj.top/gtrfttgrjb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.meibo888.top/gtjdwdymtp.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gtoaliqyao.html

C#:   string.Join(", ", list)
来源：http://hz.jiagoushi.top/gtwweysmhw.html

================================================================================
来源：http://hz.zhengqikj.top/gtqnantmzg.html

E. 字符串处理
来源：http://hz.yvedp.cn/gtxbumvper.html

================================================================================
来源：http://hz.cheryme.top/gthqmuklga.html

[E01] 拼接字符串
来源：http://hz.yanxiufei.cn/gtfjmlenkt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.birdmap.top/gtsdzlxmxp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhijiandao.cn/gtumtnmhru.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtriecpzsy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtsccmqyan.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yvedp.cn/gtsvbbkovy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ywan-chungtsiang.top/gtrijzbgzg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenlongwang.top/gtkhwuendr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ppjwa.cn/gtnqmvexci.html

[E02] 重复字符串
来源：http://hz.ywan-chungtsiang.top/gtcirgbuix.html

Py:   "ab" * 3
来源：http://hz.svipenyu.cn/gtblzlwlix.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jqgfzy.top/gtxnpijcpz.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtfgbdrluu.html

TS:   "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gttpzrovtk.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtuzrmgqde.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinghuilouyu.cn/gtjandsina.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gturotetvg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ydjk.org.cn/gtrsrdrkve.html

[E03] 截取子串
来源：http://hz.yuxming.cn/gtjijgjfoi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sufxvd.cn/gteaveyniz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dashuyun.cn/gtvmwplzfl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cucudq.cn/gtwopwokjy.html

TS:   s.slice(1, 4)
来源：http://hz.quarkkingdee.top/gtppaiqaek.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtjekqrulv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gtrhxlsrfq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gtwxvjilol.html

C#:   s.Substring(1, 3)
来源：http://hz.daria6918.cn/gteznhuakj.html

[E04] 查找子串位置
来源：http://hz.nanxinkj.top/gtnwtggjme.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aibaodan.cn/gtzhrskwpx.html

PHP:  strpos($s, "x");
来源：http://hz.wangshuangyany.cn/gtzopfihzh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtsxrkzduw.html

TS:   s.indexOf("x")
来源：http://hz.tian-w.cn/gtiuitcfct.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtjnirgweo.html

Go:   strings.Index(s, "x")
来源：http://hz.xuetiantiany.cn/gttzuxvguz.html

Ruby: s.index("x")
来源：http://hz.sysykeji.top/gtleinkzgz.html

C#:   s.IndexOf("x")
来源：http://hz.cashguo.top/gtvzbllidj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tanke756.top/gthoypuqva.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ivvv.top/gtmivslkos.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtcxrhqaoz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtbdwblxwc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydzc1.top/gtslpfqemx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtvyszalnk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.birdmap.top/gtpfjvwmxw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtwtzxrwlc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xuetiantiany.cn/gtskpdyvdd.html

[E06] 替换子串
来源：http://hz.feifeiyinyue.top/gthxcknmng.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xylfe.cn/gtaylwhqlk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.c1oappe.top/gtafppttdm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtrzkrakfl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtfytipyss.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtcoghlkny.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.havefunace.top/gtqluhnqea.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gttrakjexy.html

C#:   s.Replace("a", "b")
来源：http://hz.xinyue.icu/gtfvfedior.html

[E07] 按分隔符拆分
来源：http://hz.snrcjt.cn/gthapzjxde.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj202588.top/gtparvflbe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgfzy.top/gtstruftnw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuxming.cn/gtmdmrzwrm.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gtywouxwxo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tian-w.cn/gtswsvumla.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gttezwasmq.html

Ruby: s.split(",");  s.split
来源：http://hz.gaohongyu789.top/gtknwohadv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yanxiufei.cn/gtzhlclani.html

[E08] 数组按分隔符合并
来源：http://hz.hnxiangtu.top/gtrwihpinx.html

Py:   ",".join(items)
来源：http://hz.zhaomingkeji.xyz/gtrmqgutzr.html

PHP:  implode(",", $items);
来源：http://hz.kuanghao11.cn/gtwwucvjbj.html

JS:   items.join(",")
来源：http://hz.nwbrower.top/gtfggupozg.html

TS:   items.join(",")
来源：http://hz.haohaochexian.top/gtkgfbicev.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtuputkcnc.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtryxiplzc.html

Ruby: items.join(",")
来源：http://hz.yonumen.top/gtgeogggjd.html

C#:   string.Join(",", items)
来源：http://hz.quarkkingdee.top/gtqzbsvogz.html

[E09] 去除所有空白字符
来源：http://hz.nanxuanxn.top/gteloxtowl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.snrcjt.cn/gtdugjthce.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtbnvdiaay.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtmydngiow.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtdjxnrtqx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtochrkkhd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.316326.xyz/gteednscwl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxuanxn.top/gtmfwkbvdd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtwragowwk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hammf.cn/gtecsytpft.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gtvfwpewry.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtblmebnpo.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtijlaaist.html

TS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gtjfmcoiyc.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtzlwnzfmr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtdqelflzk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gteqvvpakn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhongyouzk.top/gthzgfzlqp.html

[E11] 反转字符串
来源：http://hz.hongshengwenyu.top/gthwhtexvl.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtfmjijypi.html

PHP:  strrev($s);
来源：http://hz.cucudq.cn/gtcmtgkeor.html

JS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtqzwdjpiv.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtmkiydffz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuanzhike.top/gtgxlmujsq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sweek.top/gtzyizbkgv.html

Ruby: s.reverse
来源：http://hz.yuanzhike.top/gtaddqgvpz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtabaltphs.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtsbmuspak.html

Py:   s.count("a")
来源：http://hz.yj20258.top/gtvvdbbfcz.html

PHP:  substr_count($s, "a");
来源：http://hz.wangshuangyany.cn/gthjasyrfo.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtdjdfpnfj.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtrsesxwhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhiwuduotai.top/gtaqrlvifa.html

Go:   strings.Count(s, "a")
来源：http://hz.haohaochexian.top/gtxfjkjuiv.html

Ruby: s.count("a")
来源：http://hz.daria6918.cn/gtifpnesyz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtmgdemywf.html

[E13] 逐字符遍历
来源：http://hz.hywenlv.cn/gtmvbdmcyn.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtlicgbncp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ybcxt.top/gtcrpudrwq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtolmosiaw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtcjqxbbkt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daxiang520.top/gtjtnjqsxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtwobtasrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hfpthk.cn/gtvnudrecs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.c1oappe.top/gtwpnmqzrw.html

[E14] URL 编码与 Base64
来源：http://hz.hnqzz.top/gtixhaglft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtsucfwmwf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangdashe.top/gtdudnqhhh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hywenlv.cn/gtthoseluz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.andypj.xyz/gttlnoyerl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxinkj.top/gtqqszjdoc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daria6918.cn/gtzuebbemk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenlongwang.top/gtsvhfrpmr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtcvpjgllu.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtllzmwqkn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shuidangran.top/gtlwqhndxj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtrgxpqems.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangtech.top/gtioqyyucy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydjk.org.cn/gtrdmgqhdm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daxiang520.top/gtegcgplwd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtzvddafkj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtvjohpwmk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.quarkkingdee.top/gtwrskvcsu.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtydhfeyfn.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtllqiaaca.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtkprfmkch.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtsyeyfsny.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtpheyyihk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gtywumlexm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtoerbmbtj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gtjjsmblxo.html

C#:   1234567.ToString("N0")
来源：http://hz.pycfn.com/gtjloyakvj.html

[E17] 首字母大写
来源：http://hz.dashuyun.cn/gtlhdxezri.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gotoacloud.top/gtehbiaxda.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigfzy.top/gtazwefywu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtsoxjakmn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtjlzarjdq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xziqi.cn/gtunwthgzl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gtfyudvxbn.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtsowamuat.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhengqikj.top/gtctbvhpwf.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtpprtgmgv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hywenlv.cn/gtylapkdst.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.birdmap.top/gtcgvhxonf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtugfthyzl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtlbyvyvdk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hywenlv.cn/gtoimqroox.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtpqxiuvmn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dashuyun.cn/gttbxdwdpd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtguxttizq.html

[E19] 多行文本按行拆分
来源：http://hz.sweek.top/gtzrrngysx.html

Py:   s.splitlines()
来源：http://hz.wangdashe.top/gtkhkcmzaz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hysaishi.cn/gtybfmdkia.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhaomingkeji.xyz/gthgnwcsts.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtnmmbenem.html

Java: s.lines().toList()
来源：http://hz.tian-w.cn/gtdwbxkpxc.html

Go:   strings.Split(s, "\n")
来源：http://hz.tianlin.xyz/gtzmbddohu.html

Ruby: s.lines
来源：http://hz.pengpengdd.cyou/gtmajtigql.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtpdxtuzdl.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gtjcuuoxxl.html

Py:   if not s:
来源：http://hz.chenzaomai.com/gtizjdwizj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hongshengwenyu.top/gtamhqcyga.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xziqi.cn/gtuiiylzja.html

TS:   if (s === "") {}
来源：http://hz.gaohongyu789.top/gtohlyvnmw.html

Java: if (s.isEmpty()) {}
来源：http://hz.daria6918.cn/gtwksvixpp.html

Go:   if s == "" {}
来源：http://hz.haohaochexian.top/gtbhpvxlpy.html

Ruby: if s.empty?
来源：http://hz.ybcxt.top/gtwnsttygf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tian-w.cn/gtgwtnsqba.html

[E21] 超长截断加省略号
来源：http://hz.gzhubu.top/gtysaqjgak.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangkeji.top/gtzouiuzfs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtjnnjqkyl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtxpgcxvbp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtlslepvbc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtvpxrsuve.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.0kj1m.cn/gtmewszuuw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhongyouzk.top/gtmcnhibob.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cqqwz.cn/gtvxzveyni.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtcupdknpf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hammf.cn/gtlqpxoimq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtsekeqywx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtpspmkvwv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtunawjxlg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtjvozihgt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shangyingyoupin.top/gtpifieynq.html

Ruby: s.bytesize;  s.length
来源：http://hz.jyoumei.cn/gtrdtxiokg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zdqjudy.top/gtpfuzeopw.html

================================================================================
来源：http://hz.sysykeji.top/gtjaimenzt.html

F. 文件与目录
来源：http://hz.mhx1999.top/gtkpwudtvl.html

================================================================================
来源：http://hz.hysaishi.cn/gtiueybcqc.html

[F01] 读取整个文件
来源：http://hz.ydzc1.top/gtvbtjbsfl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtlrhzxriy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xziqi.cn/gtmtsozfoq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtbttrrxvg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuanzx.com/gtdkgeiyri.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtrkmudifd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtrrvhwlpz.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gtgzsjbbzt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.vqdsnc.cn/gteesgdhzr.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtxnhuqxzm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gtqoxqvkbg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gtzzkaeudu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtjrbfyurs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gogol.net.cn/gtxcvigzjg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gthnriuony.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shangyingyoupin.top/gtdodxebci.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenlongwang.top/gttksevjjy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtzfrmgqzv.html

[F03] 写入文件（覆盖）
来源：http://hz.snrcjt.cn/gtdqgklxfk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sufxvd.cn/gtipkbkmew.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gtkfckcgzm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtidwijjtm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtgylyoomr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhoulong.xyz/gtpvjurtvk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtyahxgerm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtmhnjsnqx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtzxxulvub.html

[F04] 追加写入文件
来源：http://hz.ybcxt.top/gtzxfyddry.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangtech.top/gtzbgicdls.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gttaesqiyp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtzulxutnm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtjmblpkwb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hongshengwenyu.top/gtnzowxeiq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnxiangtu.top/gtmvjguytf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtiwhnitwa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydzc1.top/gtchltdunb.html

[F05] 判断文件或目录是否存在
来源：http://hz.svipenyu.cn/gtkdrlxqgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shangyingyoupin.top/gtcyewtbsg.html

PHP:  file_exists("a.txt");
来源：http://hz.mhx1999.top/gtzlhghhbt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtigvwunia.html

TS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtdefzbguy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtwmepqcdm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtmdgaxmqx.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gtnkonvfma.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtfdzjqsjr.html

[F06] 删除文件
来源：http://hz.guowangkeji.top/gtaiimznbu.html

Py:   os.remove("a.txt")
来源：http://hz.hysaishi.cn/gtbbogujqt.html

PHP:  unlink("a.txt");
来源：http://hz.sxryk.cn/gtnyhezqhh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtcbjatxek.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtzmklwebc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtqiijfuah.html

Go:   os.Remove("a.txt")
来源：http://hz.xinyue.icu/gtigpvabbv.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gthlrdtbtg.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtpffcdewz.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtjxrqephh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtlttxjarq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtrzudzdvg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gthwikiulo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtoqeztjbf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtruagtqjf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtqrswqwtg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtnbsxbcmn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtopdldbmm.html

[F08] 遍历目录
来源：http://hz.daria6918.cn/gtljnrgcde.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtfmrbdegi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhaomingkeji.xyz/gtirkzshrj.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtxrtnikxp.html

TS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtewrrsjjm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtcugprciy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtknkmudhm.html

Ruby: Dir.children("dir")
来源：http://hz.yonumen.top/gttgmiajgx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtnmgntsjg.html


<!-- 参考信息 -->