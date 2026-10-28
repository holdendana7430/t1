代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cucudq.cn/gtxqknsawe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtwazgewix.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yvedp.cn/gtvwmipiza.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtcewzutou.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gotoacloud.top/gtnylugnzm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.smart0.xyz/gtqypofuhv.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigufen.top/gtpdzrwgcz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hongshengwenyu.top/gtfctqqkcs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cqqwz.cn/gttwotzroo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.andypj.xyz/gtjxgfhvil.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shangyingyoupin.top/gtvkfavalj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jiagoushi.top/gtqjzntvjk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtwrdsowxl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenlongwang.top/gtpdtmmwsn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigfzy.top/gtsbatkuny.html

[D26] 数组转字符串
来源：http://hz.gogol.net.cn/gtstxlattt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aizwys.cn/gtjtetgjou.html

PHP:  implode(", ", $arr);
来源：http://hz.yangfankeji.com/gtgtklepjv.html

JS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gtciiilamr.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtavolzysk.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtmszzjcak.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinyuanbaomall.cn/gtkbvcvuzl.html

Ruby: arr.join(", ")
来源：http://hz.fengsongda.top/gtxbppmrfr.html

C#:   string.Join(", ", list)
来源：http://hz.shangyingyoupin.top/gteqsrpcda.html

================================================================================
来源：http://hz.dianchejie.cn/gtvfashzje.html

E. 字符串处理
来源：http://hz.sysykeji.top/gtyxxtewtr.html

================================================================================
来源：http://hz.cdnleiting.top/gtyvelewol.html

[E01] 拼接字符串
来源：http://hz.yuanzhike.top/gtbgvfbums.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtwksdnmvs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenzaomai.com/gtscabbexh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtsroiumjp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtlkoxclzi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhijiandao.cn/gthdofixml.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhiwuduotai.top/gtfclhssno.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gtcrtnqpbj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sysykeji.top/gtluwlzkxa.html

[E02] 重复字符串
来源：http://hz.chenjidiqi.icu/gtzelojroj.html

Py:   "ab" * 3
来源：http://hz.hnqzz.top/gtszysimzk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnqzz.top/gtriahdtpa.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtqtmdjiib.html

TS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtagzgbpxn.html

Java: "ab".repeat(3)
来源：http://hz.birdmap.top/gtjoovfelr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.bjfxy.top/gtkwuvmdyt.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtzjjvoaop.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtgwdcfqle.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gtgjztjtyq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sweek.top/gtwhtivkic.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.smart0.xyz/gtuzyqykho.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtbpmnbvwy.html

TS:   s.slice(1, 4)
来源：http://hz.xziqi.cn/gtsotxymav.html

Java: s.substring(1, 4)
来源：http://hz.pycfn.com/gthltnsghb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtmptkryue.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tianlin.xyz/gtirrerpxw.html

C#:   s.Substring(1, 3)
来源：http://hz.jianghu66.top/gtnmjbtxzy.html

[E04] 查找子串位置
来源：http://hz.cqqwz.cn/gtlqercfyp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gotoacloud.top/gthsvukfur.html

PHP:  strpos($s, "x");
来源：http://hz.yj202588.top/gtuvknderu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydjk.org.cn/gtrnjhcrxk.html

TS:   s.indexOf("x")
来源：http://hz.meibo888.top/gtfmllqcht.html

Java: s.indexOf("x")
来源：http://hz.aizwys.cn/gtefvpjlgm.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtqqahafqm.html

Ruby: s.index("x")
来源：http://hz.ivvv.top/gtdhxhgdmv.html

C#:   s.IndexOf("x")
来源：http://hz.meibo888.top/gtewefwvfq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sufxvd.cn/gtnxtompmr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhijiandao.cn/gtopltnfnk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydjk.org.cn/gthunnmkuh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtgovgofci.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtercscqjd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yangfankeji.com/gtctsolpqi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtmetxuxwd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.haohaochexian.top/gtkddzyedh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zdqjudy.top/gtwvbrwuya.html

[E06] 替换子串
来源：http://hz.yj202588.top/gtpxfhwige.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgufenzy.top/gtcofwzawa.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinqigufen.top/gtjzljxoss.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtmjhhowll.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtklamlfsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gthtudjxpq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenzaomai.com/gtfnhzevjh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhengqikj.top/gtnfvengyn.html

C#:   s.Replace("a", "b")
来源：http://hz.ivvv.top/gtsexeschw.html

[E07] 按分隔符拆分
来源：http://hz.jqgfzy.top/gtgxpftgzn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gtklzaozsc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtxmpmjwsz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtiitucvjj.html

TS:   s.split(",")
来源：http://hz.mhx1999.top/gtlfcjxiec.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtdonjtrca.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.0kj1m.cn/gttlikglnf.html

Ruby: s.split(",");  s.split
来源：http://hz.sweek.top/gtlgpzycrk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtdbxvlafb.html

[E08] 数组按分隔符合并
来源：http://hz.gzhubu.top/gtiiujpfpc.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gtjhgmxblr.html

PHP:  implode(",", $items);
来源：http://hz.ydjk.org.cn/gtehmstvwb.html

JS:   items.join(",")
来源：http://hz.fzhhl.top/gtmfayudxd.html

TS:   items.join(",")
来源：http://hz.tanke756.top/gtwbvvvaml.html

Java: String.join(",", items)
来源：http://hz.0kj1m.cn/gtohxqxstu.html

Go:   strings.Join(items, ",")
来源：http://hz.fengsongda.top/gtcexmnvwa.html

Ruby: items.join(",")
来源：http://hz.xinyue.icu/gtrndzohyc.html

C#:   string.Join(",", items)
来源：http://hz.quarkkingdee.top/gtcjrkgcly.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gtjzdseoqd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtftgemblm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtucpqrsxc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtonmupvwa.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtpdjkdcpm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtnyrqpket.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtcnwjyuit.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guannengcc.top/gtgahtddnp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gtdtdedsqk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258888.top/gtumpdmnva.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtobymgarf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtxuxlwruq.html

JS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtupvwtyni.html

TS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtsxcbylzd.html

Java: String.format("%03d", 7)
来源：http://hz.yonumen.top/gttkrbsmfn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtoimntisw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtxcfutoou.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtcwdxgael.html

[E11] 反转字符串
来源：http://hz.316326.xyz/gtogthnzgb.html

Py:   s[::-1]
来源：http://hz.nanxuanxn.top/gtgulehvbb.html

PHP:  strrev($s);
来源：http://hz.nwbrower.top/gtkcyyspyx.html

JS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtlvqsjehp.html

TS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtxcvqkadt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtsctbcdxs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tian-w.cn/gtarzmguiy.html

Ruby: s.reverse
来源：http://hz.shanyushiyangtech.top/gtizwkxtuu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtkgovsfjj.html

[E12] 统计某字符出现次数
来源：http://hz.zhixingplan.top/gtoxprxopl.html

Py:   s.count("a")
来源：http://hz.jinghuilouyu.cn/gtcykmblgc.html

PHP:  substr_count($s, "a");
来源：http://hz.yanxiufei.cn/gtfpsynnhs.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtjzmjvgix.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtndtytfbh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtkowyxniy.html

Go:   strings.Count(s, "a")
来源：http://hz.dianchejie.cn/gtqqvkxbrs.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtmrlhyafu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yvedp.cn/gtlxdeeebp.html

[E13] 逐字符遍历
来源：http://hz.aizwys.cn/gtkspytjpz.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtjkozuwht.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtdioznbkk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtnekcqnbc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtvufnchmu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxuanxn.top/gthjgromoc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gtednxpffe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ehwqpu.com/gtxqukfyqj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtevzouqkz.html

[E14] URL 编码与 Base64
来源：http://hz.feifeiyinyue.top/gtgcprapzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.c1oappe.top/gtmrdbayeb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtkyzhkhuy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guowangkeji.top/gtjfclvyrj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gaohongyu789.top/gtegxbrohw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pycfn.com/gtawbfcxtq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258888.top/gtculefhkn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtpjfudtyr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtwqnxxdbu.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258888.top/gtmoqkblmh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hywenlv.cn/gtwgsqbjbf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hysaishi.cn/gttdrtthss.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ywan-chungtsiang.top/gthzgbvipp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gtmcecobdh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgfzy.top/gtctcqrpyt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gtherdarup.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gtgqdchhyk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.9152youxi.cn/gtdxastrls.html

[E16] 数字千分位
来源：http://hz.dianchejie.cn/gtdgegibsd.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtwmjafnym.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gtwvbneeef.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtkfucvswg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtootcrqwl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gzhubu.top/gtimtwrbie.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtsbainvun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangkeji.top/gtciqsqsot.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtvzhrbrqh.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtemwshmmh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtrjgocihr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtfgdtfjbn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtcnzwxopp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtxalldpss.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jianghu66.top/gtwdesrdza.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.bjfxy.top/gtjtibokgg.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtnuvzikqo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yongpay.top/gtsazgvfbh.html

[E18] 模板占位符替换
来源：http://hz.xingfuxueyuan.xyz/gtgueoqmvm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtovstehom.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhaomingkeji.xyz/gtchvjlrun.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtsijrgttm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gthsmdtrlm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtindacanx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sweek.top/gtttufgfoh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenjidiqi.icu/gtfguconow.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtmletfgmt.html

[E19] 多行文本按行拆分
来源：http://hz.xuanzx.com/gtutxgyyxv.html

Py:   s.splitlines()
来源：http://hz.jlsjyb.cn/gtvbqzzcnj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sufxvd.cn/gtnbyrixxs.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtwcmoacqt.html

TS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtxkpfbcja.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtubqazrce.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtduwnpnuc.html

Ruby: s.lines
来源：http://hz.chenzaomai.com/gtkoyqophq.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtmufukwln.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtlclcowls.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtqczdpkcp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tian-w.cn/gtoginfazb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.c1oappe.top/gtcjtadbmt.html

TS:   if (s === "") {}
来源：http://hz.zhixingplan.top/gtgvoblhma.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtvpsheqmt.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtxpudpthg.html

Ruby: if s.empty?
来源：http://hz.ydzc1.top/gtkyqgerkx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fzhhl.top/gtszhwylwt.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gtrpxngqbf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gogol.net.cn/gtrglfopdt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.svipenyu.cn/gtmwcfvpmh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtvlnqvngr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gthaieicqw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gthyozbspn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtllrbprln.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtdakidtcz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtnrktfayt.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gtfglhisxn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinghuilouyu.cn/gtwbxtzpah.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gthcbqjqas.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtqcjnqfdu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtneoxwvgc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gtnwlxndwa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gtvwmaikuj.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtggwhkyhj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yongpay.top/gtgupppuoe.html

================================================================================
来源：http://hz.dianchejie.cn/gtflzymvop.html

F. 文件与目录
来源：http://hz.daxiang520.top/gtaoyzlrwu.html

================================================================================
来源：http://hz.ivvv.top/gtlrvstehk.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtlpsjmxep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sweek.top/gtnvcykfco.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ppjwa.cn/gtpmurrnmq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gtsvufetpr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxinkj.top/gtqgsvzqss.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtprmxtfqq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yongpay.top/gtyjrixuve.html

Ruby: File.read("a.txt")
来源：http://hz.quarkkingdee.top/gtqohkngfw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jiagoushi.top/gtvqwwjwne.html

[F02] 逐行读取文件
来源：http://hz.zhixingplan.top/gtnxdqxoul.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtrbmklhsj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtigcisurm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtekpqsxpr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtnmenrhoa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtsiiaivdm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shuidangran.top/gtssbfzpvf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ehwqpu.com/gtuxsssyzk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtgfbfxsqy.html

[F03] 写入文件（覆盖）
来源：http://hz.yonumen.top/gtiaoguboq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gtgkkmgxxg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtxpvmwkrp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtxgffitiq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hammf.cn/gtcaciatxn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtsgrnjfvv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ppjwa.cn/gtjfnpmiqh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dianchejie.cn/gtidxexcmc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yueranfly.top/gtufzdacgm.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtnlcdykmc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gtlirfmyam.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtqzfjzhfv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtqpoedeqj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtqhmvdvhv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtnuhqbprl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtzkqqsmlz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtmzhshzth.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sweek.top/gtrnrjvckm.html

[F05] 判断文件或目录是否存在
来源：http://hz.havefunace.top/gtwmigloxq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258.top/gtrtozrrbe.html

PHP:  file_exists("a.txt");
来源：http://hz.yueranfly.top/gtshdeuhan.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gthhgrdhpm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtcxazdobx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtsmtmccxi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhaomingkeji.xyz/gtnmprjfrg.html

Ruby: File.exist?("a.txt")
来源：http://hz.nwbrower.top/gtustbdpfk.html

C#:   File.Exists("a.txt")
来源：http://hz.svipenyu.cn/gtbaadxxbt.html

[F06] 删除文件
来源：http://hz.yonumen.top/gtvcvmzkyn.html

Py:   os.remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtpfenqusa.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtezydthty.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtflkintxc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtfuyouxhg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gteenectni.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtqammoane.html

Ruby: File.delete("a.txt")
来源：http://hz.quarkkingdee.top/gtocebkbih.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gtelaojbst.html

[F07] 创建目录（含多级）
来源：http://hz.sufxvd.cn/gtdqaffauo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnxiangtu.top/gtpvsuyxyu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yonumen.top/gtuormazzg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtwlffoctm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gteikbneas.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daria6918.cn/gtymfchahe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cdnleiting.top/gtfafwayij.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenzaomai.com/gtalrxnsem.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.kuanghao11.cn/gtmzlgrsmg.html

[F08] 遍历目录
来源：http://hz.guannengcc.top/gtzrednfis.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zdqjudy.top/gtfuehqvok.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhixingplan.top/gtenrisgjo.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtwjovlnxv.html

TS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtxsklyrik.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtpohfhpuh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhijiandao.cn/gtwasnljsr.html

Ruby: Dir.children("dir")
来源：http://hz.redwolf501.top/gtpcjaahdc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtglypahvy.html


<!-- 参考信息 -->