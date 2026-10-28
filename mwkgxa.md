代发 wailian999

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gtsrnxywkl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.kuanghao11.cn/gtmgppteue.html

[D21] 判断是否包含某元素
来源：http://hz.hywenlv.cn/gtyhggjiaz.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtqogskgoa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ivvv.top/gtrdrbtxsi.html

JS:   arr.includes(x)
来源：http://hz.xinyue.icu/gthvumilci.html

TS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtfndglyvx.html

Java: list.contains(x)
来源：http://hz.shanyushiyangtech.top/gtmcukplnl.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtdqvduvoo.html

Ruby: arr.include?(x)
来源：http://hz.shzxlz.cn/gtsmmsaabd.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gtlkcnvjbp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hongshengwenyu.top/gtjmlryiiw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtkoamvmha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yvedp.cn/gtliwdixit.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtnjnafegg.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtydygbytn.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtotlqfdmf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtzarkmcnd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cheryme.top/gtlvfbmhiq.html

C#:   new List<int>(list);
来源：http://hz.snrcjt.cn/gtrgvqevxg.html

[D23] reduce 累积计算
来源：http://hz.c1oappe.top/gtqpbzrpib.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cheryme.top/gtbhdpsbpz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gtrhcuhwlx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtagpstvvo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtnictiotd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.kuanghao11.cn/gtbkcoxuyp.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtpingklze.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.snrcjt.cn/gtbpawjlii.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.svipenyu.cn/gtonvudlsd.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgufenzy.top/gtyqutmvie.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtayadqaci.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydjk.org.cn/gtrdxumwbg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigufen.top/gtajkviari.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtjkuiqyjm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangshuangyany.cn/gtmbztvnuw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yueranfly.top/gtydfgucjs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtkmrsebfr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ywan-chungtsiang.top/gtektftvti.html

[D25] Set 集合去重与交并差
来源：http://hz.xingfuxueyuan.xyz/gthyottflp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tanke756.top/gttuwiccgk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aibaodan.cn/gtegckyjzw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangshuangyany.cn/gtjpmekioh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shuidangran.top/gtyzdoopkf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxinkj.top/gtepyixzar.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtygqucphq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yueranfly.top/gtgbgbhqku.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shzxlz.cn/gtijazbjwd.html

[D26] 数组转字符串
来源：http://hz.316326.xyz/gtiimgpyoc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuanzx.com/gtvwcsdfpy.html

PHP:  implode(", ", $arr);
来源：http://hz.sufxvd.cn/gtkcutofkk.html

JS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtxzuybnkf.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtvcyglngi.html

Java: String.join(", ", list)
来源：http://hz.dashuyun.cn/gtbuprbpno.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhaomingkeji.xyz/gthxclbjwn.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gthhggwsgz.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gtrjckdchd.html

================================================================================
来源：http://hz.0kj1m.cn/gtuxendgep.html

E. 字符串处理
来源：http://hz.vqdsnc.cn/gtfmbacopr.html

================================================================================
来源：http://hz.yj20258888.top/gthghtnnos.html

[E01] 拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtugjljplx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xylfe.cn/gtefsdqyzn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sufxvd.cn/gtoymumuzu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtbooakmpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtrufkwqew.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinyuanbaomall.cn/gtdugevdys.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.iojbl.cn/gtdixcuyqt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hammf.cn/gtqeznsahf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigfzy.top/gthfjpuopf.html

[E02] 重复字符串
来源：http://hz.0kj1m.cn/gtoodtnsub.html

Py:   "ab" * 3
来源：http://hz.meibo888.top/gtmydkgmpy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258.top/gtwtvgfhoy.html

JS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtrmzmblav.html

TS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gthctlwrai.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gthlztkjjq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tianlin.xyz/gtgrcslify.html

Ruby: "ab" * 3
来源：http://hz.zhijiandao.cn/gtmgutvlfb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.316326.xyz/gttzerjljh.html

[E03] 截取子串
来源：http://hz.ydjk.org.cn/gtndendljx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fengsongda.top/gthredduxt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigfzy.top/gtkvjhjxrm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pengpengdd.cyou/gtmbzgwjvj.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtaepunkcu.html

Java: s.substring(1, 4)
来源：http://hz.cashguo.top/gtyburgmdu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhijiandao.cn/gtzvqokstr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yongpay.top/gthifebjfx.html

C#:   s.Substring(1, 3)
来源：http://hz.fengsongda.top/gtdvvimwyh.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangtech.top/gthvtwmftd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangdashe.top/gtyirrptvi.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtscaiqofb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangkeji.top/gtccogmcyb.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtqsiwwuiq.html

Java: s.indexOf("x")
来源：http://hz.redwolf501.top/gtevbtvnzi.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gtecoxedqg.html

Ruby: s.index("x")
来源：http://hz.316326.xyz/gtzrxkjnzv.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtjaidwtdk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cucudq.cn/gtymurhfmh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sufxvd.cn/gtzwrdgtfw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenzaomai.com/gtpgeijsut.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtqxjeyypw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fzhhl.top/gtsryklpao.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtjbdkwyba.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.9152youxi.cn/gtujwvthho.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtqzhdwojo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shzxlz.cn/gtzpiibgec.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtdllvaett.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtvvuqmlhi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tianlin.xyz/gtzndkzzuy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtagmuwsxl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtjgenumjo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtdxqisice.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hysaishi.cn/gtzksajxbc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuanzhike.top/gtvtmygkci.html

C#:   s.Replace("a", "b")
来源：http://hz.hywenlv.cn/gtoarhobrk.html

[E07] 按分隔符拆分
来源：http://hz.jinyuanbaomall.cn/gtzmmvugio.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuanzx.com/gtgdjafymf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtjqtgyowd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.dashuyun.cn/gtqnlkmpbs.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtrswcfbva.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cdnleiting.top/gthbcbhlsj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shangyingyoupin.top/gtllwqblwg.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtruagkstt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.havefunace.top/gtufbhdauo.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gtcjclwihd.html

Py:   ",".join(items)
来源：http://hz.chenjidiqi.icu/gtrriblyqx.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtxazflfof.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtsluteoyr.html

TS:   items.join(",")
来源：http://hz.gotoacloud.top/gtewalqtcj.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gtfypfmifw.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtepfqorxb.html

Ruby: items.join(",")
来源：http://hz.fzhhl.top/gtbhmjwode.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtyblllwnb.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangkeji.top/gtlsusavwv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtwjnuhjvx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gtudwyhede.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gtghnexlcg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtdzniqnlp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangdashe.top/gtyfynslhq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtfvvgsrzb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jianghu66.top/gtbyeuoxbj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gaohongyu789.top/gtqncsbkvv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gtvidfkuau.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.snrcjt.cn/gtwcdwirxx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pengpengdd.cyou/gtukjijizk.html

JS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtxpljcegl.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtpejeprqe.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gteqdbtgev.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yueranfly.top/gtbyocljlt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jlsjyb.cn/gthiqernrv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj20258888.top/gtseaombqa.html

[E11] 反转字符串
来源：http://hz.aizwys.cn/gtweuyuwjo.html

Py:   s[::-1]
来源：http://hz.guannengcc.top/gtchpktdww.html

PHP:  strrev($s);
来源：http://hz.yuxming.cn/gtqfjwtyek.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtltomszgb.html

TS:   [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtkjgshpkj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtktdkpush.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shzxlz.cn/gtlxwjyihq.html

Ruby: s.reverse
来源：http://hz.shzxlz.cn/gtwjmqulhs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtchicwxsi.html

[E12] 统计某字符出现次数
来源：http://hz.vqdsnc.cn/gteflkfmio.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtacsueiml.html

PHP:  substr_count($s, "a");
来源：http://hz.sweek.top/gtshtvmnav.html

JS:   s.split("a").length - 1
来源：http://hz.zhongyouzk.top/gtgjfcwfxm.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtvrgdzlhe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pycfn.com/gtdwflpben.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gtspslexko.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gtasfnmbjw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sxryk.cn/gtycdjfcjj.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gthxgvxjlq.html

Py:   for ch in s: print(ch)
来源：http://hz.aizwys.cn/gtiuciljne.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhongyouzk.top/gtztdgezkf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtztiagkeg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtcbhqepjg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtbuvqlpqm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtlyjjlmza.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gtbiekzeqv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dashuyun.cn/gtmtjrkyuj.html

[E14] URL 编码与 Base64
来源：http://hz.shzxlz.cn/gtwzyomsse.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtjgbjtphb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daria6918.cn/gtlumuizmc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuanzx.com/gtkypjavgc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuetiantiany.cn/gtyyqignfg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.316326.xyz/gtzwdyhaud.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nwbrower.top/gtzkpvynvv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtcarecqex.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xziqi.cn/gtxcndevtg.html

[E15] HTML 转义 / 反转义
来源：http://hz.andypj.xyz/gtycvimyty.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pengpengdd.cyou/gtupqvmrng.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pengpengdd.cyou/gtmevizbdm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuxming.cn/gtljfwrlru.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtbkjmjane.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gtqivdxzyw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xinyue.icu/gtgtyfjawr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.redwolf501.top/gtmuhcrays.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gtjzeyhsbz.html

[E16] 数字千分位
来源：http://hz.chenzaomai.com/gtkokofjxx.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtnxukufie.html

PHP:  number_format(1234567);
来源：http://hz.ivvv.top/gtcxrpimal.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gthavkflpl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtdrpcbiyd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shuidangran.top/gtjpmvfbuy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.iojbl.cn/gttirbcrtg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shuidangran.top/gtijitzksl.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtvfyhyyaf.html

[E17] 首字母大写
来源：http://hz.tanke756.top/gtjwxdjyqf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hammf.cn/gtqbbpnwkf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtuqpilerc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtghxaaznu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtcxkipyzt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenzaomai.com/gtkycvinjg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtkestzulh.html

Ruby: s.capitalize
来源：http://hz.ywan-chungtsiang.top/gtijhvpsqk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.haohaochexian.top/gtdgcolstd.html

[E18] 模板占位符替换
来源：http://hz.nanxinkj.top/gttfdzrqux.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yvedp.cn/gtnsxziybg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xinyue.icu/gtlbvdjtou.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtexpaayql.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtfjuhdgek.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtfbqinihi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hfpthk.cn/gthgznppom.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yonumen.top/gtzivpczga.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.redwolf501.top/gtrfnsjjra.html

[E19] 多行文本按行拆分
来源：http://hz.pycfn.com/gtdoqqlrfm.html

Py:   s.splitlines()
来源：http://hz.ydzc1.top/gtyrvkxbxz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtsxyivhwg.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtkozazfkg.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtalnovjxz.html

Java: s.lines().toList()
来源：http://hz.tanke756.top/gtqzzpobix.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtklidoiyz.html

Ruby: s.lines
来源：http://hz.ywan-chungtsiang.top/gtpunsmijz.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gttyrjytyb.html

[E20] 判断字符串是否为空
来源：http://hz.hongshengwenyu.top/gtqddtndpd.html

Py:   if not s:
来源：http://hz.yj202588.top/gtgrpkwini.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtpqtjtipd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ppjwa.cn/gtlcvolccu.html

TS:   if (s === "") {}
来源：http://hz.jyoumei.cn/gtrlhfhgac.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gttrlsscdh.html

Go:   if s == "" {}
来源：http://hz.chenzaomai.com/gtgmasqkxy.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtfawvindl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gtwjcpvffs.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtvbofkiww.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ppjwa.cn/gtbgyvjtfe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtnywexbos.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gthidnzztn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtxfoqduwt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtmjwbdakv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.c1oappe.top/gtmgqxnwnn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtzyohtmzj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtexwodtmx.html

[E22] 字节长度与字符长度
来源：http://hz.cashguo.top/gtnxxnnprj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gtvcagedcq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtvijwxykg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtotuchyre.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtlmqjaadp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtxsiazppm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtrdfddnrt.html

Ruby: s.bytesize;  s.length
来源：http://hz.hongshengwenyu.top/gtwflkzkiu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtfjvfrhwc.html

================================================================================
来源：http://hz.yuxming.cn/gtcewqnepa.html

F. 文件与目录
来源：http://hz.quarkkingdee.top/gtgmncimho.html

================================================================================
来源：http://hz.cashguo.top/gtczhhpmmb.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtdvvbbaya.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shangyingyoupin.top/gtlevtpgcc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuanzhike.top/gtlfnziyqc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtrwqmisag.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hongshengwenyu.top/gtdjwigogy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtebxltlop.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenjidiqi.icu/gtcucxviwn.html

Ruby: File.read("a.txt")
来源：http://hz.52xcode.cn/gtybktflky.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangdashe.top/gttjyrjqvb.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtkwkeingb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jyoumei.cn/gtyccuxpjp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gtumwgchsp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtutjrcjkc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtnlsrskyd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtkdtspozj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgfzy.top/gteygqrzdi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangtech.top/gtenjgkzyx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gtqfzgxcfe.html

[F03] 写入文件（覆盖）
来源：http://hz.0kj1m.cn/gtnpbdtynb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnxiangtu.top/gtjilzciog.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtbvjemhhi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuetiantiany.cn/gttlrdepaa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtmxvpvzrl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gttoeivrcc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtoidiwijh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtpbhbxemo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtibyjzokt.html

[F04] 追加写入文件
来源：http://hz.yuanzhike.top/gtqkeyathj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cashguo.top/gtarjbksdj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pycfn.com/gtwqhefrxx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtsrrmiifu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtmaqeauvx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gthcnkjstu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtbcmckcwj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtypllxaan.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtjduetvjo.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gtwywoemzz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhixingplan.top/gtrwecoxil.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gtuuyzxpqw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.0kj1m.cn/gtytvxethc.html


<!-- 参考信息 -->