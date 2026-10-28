代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtwsjgpiqf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtgvnneork.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yueranfly.top/gtljniegaf.html

Go:   // 手写 map[T]int
来源：http://hz.pengpengdd.cyou/gtputyqdqp.html

Ruby: arr.tally
来源：http://hz.andypj.xyz/gtezbgtuez.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.c1oappe.top/gtntuypwcq.html

[D21] 判断是否包含某元素
来源：http://hz.cucudq.cn/gtdhhvvkud.html

Py:   x in arr
来源：http://hz.ydjk.org.cn/gtxstlzfxn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zdqjudy.top/gtfxgiblpf.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtropqksui.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gtbwutyhcj.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtbvenyvep.html

Go:   slices.Contains(arr, x)
来源：http://hz.316326.xyz/gtrqanuacx.html

Ruby: arr.include?(x)
来源：http://hz.ehwqpu.com/gtngahfphm.html

C#:   list.Contains(x)
来源：http://hz.yonumen.top/gtdtbxzdoh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xziqi.cn/gtlhsecdtd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtbgwmpunb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.dianchejie.cn/gtsfvxfzqw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gtbssozhfh.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gtzwtbfbzu.html

Java: new ArrayList<>(list);
来源：http://hz.zhijiandao.cn/gtdfbottgl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigfzy.top/gttxgmyifi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yueranfly.top/gtqdroicvo.html

C#:   new List<int>(list);
来源：http://hz.xylfe.cn/gtkawfdmig.html

[D23] reduce 累积计算
来源：http://hz.ydzc1.top/gtdcxficex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtpptqzzzl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.andypj.xyz/gtfrbswpnk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtnpwxdadf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtgwlwjnmh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtjsrvhxef.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtibporscw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ybcxt.top/gtfeesrves.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinyuanbaomall.cn/gtjzyuitmm.html

[D24] 字典 / Map 基本操作
来源：http://hz.daxiang520.top/gtsyxriown.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gtqtwjvktx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtsuiruttp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jianghu66.top/gtsttielok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sysykeji.top/gtlmrwlpdu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gotoacloud.top/gtdkdxsuxp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtqukaikpx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gtgvnlxusn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ivvv.top/gtdontcerg.html

[D25] Set 集合去重与交并差
来源：http://hz.yuanzhike.top/gtynaisfln.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xingfuxueyuan.xyz/gtbltnekfa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.quarkkingdee.top/gtgazlkoms.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cdnleiting.top/gtughuwgir.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xingfuxueyuan.xyz/gtdiellfbv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtjgfgpoxl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtmwpwiadr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cqqwz.cn/gtofjghgkg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinghuilouyu.cn/gtpmufadyo.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gttoixthah.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtzfqlihgd.html

PHP:  implode(", ", $arr);
来源：http://hz.c1oappe.top/gtpbdokqcb.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtnmitgsbo.html

TS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtfgqsipqi.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtianefbrs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtkcwvjeqh.html

Ruby: arr.join(", ")
来源：http://hz.ydzc1.top/gtwfzvbcjx.html

C#:   string.Join(", ", list)
来源：http://hz.xylfe.cn/gtzfkmntbf.html

================================================================================
来源：http://hz.gogol.net.cn/gthntdaphm.html

E. 字符串处理
来源：http://hz.0kj1m.cn/gtccdmhebm.html

================================================================================
来源：http://hz.yj20258.top/gtkfvmxoto.html

[E01] 拼接字符串
来源：http://hz.xylfe.cn/gtwwmrquab.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cqqwz.cn/gtgkpauvlk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gthtbzvhgk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtmxglbron.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.feifeiyinyue.top/gtdslugfeq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cheryme.top/gtvwsptozf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hfpthk.cn/gttbznsbxa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xinyue.icu/gtomugyewn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cheryme.top/gtqbhdesme.html

[E02] 重复字符串
来源：http://hz.jiagoushi.top/gtoibvcmuj.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtmpbffrbp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangshuangyany.cn/gtdhqskrfe.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtqsbzsqnk.html

TS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtquvvxsuq.html

Java: "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtozvkptdz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtasnsjrfq.html

Ruby: "ab" * 3
来源：http://hz.kuanghao11.cn/gtzaxfywht.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtjwysxwig.html

[E03] 截取子串
来源：http://hz.gotoacloud.top/gtzssnsfia.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtcwurdkoh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258.top/gtbhkiiegf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydzc1.top/gttnxigrln.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigufen.top/gtedlwpnwy.html

Java: s.substring(1, 4)
来源：http://hz.ppjwa.cn/gthzwhwjak.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.52xcode.cn/gtwrdsettn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtaaivaamd.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtwhzgrdgn.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gtacajyymr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtvrkueudl.html

PHP:  strpos($s, "x");
来源：http://hz.yueranfly.top/gttfzicaas.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fengsongda.top/gtdaazdclk.html

TS:   s.indexOf("x")
来源：http://hz.chenlongwang.top/gtnbunxxzz.html

Java: s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtnvfwaril.html

Go:   strings.Index(s, "x")
来源：http://hz.jianghu66.top/gtmmwiqoxp.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtmxaitihz.html

C#:   s.IndexOf("x")
来源：http://hz.gzhubu.top/gtwrvqtpzw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.haohaochexian.top/gtclealmef.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ppjwa.cn/gtdnieleym.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ppjwa.cn/gtrjpysywz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gtvwqlctaw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jyoumei.cn/gtunxhgnmx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtdqycjpty.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fengsongda.top/gtokrntzif.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtqtozmmtm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.snrcjt.cn/gtizfzzwfu.html

[E06] 替换子串
来源：http://hz.jqgufenzy.top/gtjfhdrpte.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtzptryqri.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gttjwteduq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtivxpgaqg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtemkbuxex.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtkuedaply.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.svipenyu.cn/gtngjoeyrl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ppjwa.cn/gtggoxtelu.html

C#:   s.Replace("a", "b")
来源：http://hz.haohaochexian.top/gtitmqplrt.html

[E07] 按分隔符拆分
来源：http://hz.fengsongda.top/gtczkjkybk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.quarkkingdee.top/gtdlbbbstv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenlongwang.top/gtgxjldonk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.9152youxi.cn/gtarywahea.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gthvtgpobj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gtznafrqfy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hongshengwenyu.top/gtrncizrdu.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtrkzeqwwh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.iojbl.cn/gtmkmtlgdt.html

[E08] 数组按分隔符合并
来源：http://hz.shanyushiyangkeji.top/gtpvwaqude.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtiyjrxntq.html

PHP:  implode(",", $items);
来源：http://hz.chenzaomai.com/gtlamfkjkf.html

JS:   items.join(",")
来源：http://hz.daxiang520.top/gtxqpkoxhx.html

TS:   items.join(",")
来源：http://hz.xinyue.icu/gtxnozllor.html

Java: String.join(",", items)
来源：http://hz.dashuyun.cn/gtjuircgxq.html

Go:   strings.Join(items, ",")
来源：http://hz.hysaishi.cn/gtalbudwbi.html

Ruby: items.join(",")
来源：http://hz.tian-w.cn/gtxwrzcaxk.html

C#:   string.Join(",", items)
来源：http://hz.hysaishi.cn/gtepbzlklu.html

[E09] 去除所有空白字符
来源：http://hz.jinghuilouyu.cn/gtpizagpxv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sxryk.cn/gtfmxtlayv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yuanzhike.top/gtokcmlxbq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtyrngoxkn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sufxvd.cn/gtjslrxqjq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhongyouzk.top/gtkbhtrntn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtvwmszfwy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jiagoushi.top/gtgatfdsiq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cdnleiting.top/gtwucldtyu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.52xcode.cn/gtulscfezy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtonueuajd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ybcxt.top/gtnsriygwo.html

JS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtfpyvtubm.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtbdwnolzd.html

Java: String.format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtumhslomm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtxkijwabx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtoftfntnb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhiwuduotai.top/gtqshnrcyv.html

[E11] 反转字符串
来源：http://hz.haohaochexian.top/gtqrjsatht.html

Py:   s[::-1]
来源：http://hz.tian-w.cn/gtvorzrqii.html

PHP:  strrev($s);
来源：http://hz.snrcjt.cn/gtiiuktnmn.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtvjpeqzie.html

TS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gttvsemwlp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gttlioobtb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinghuilouyu.cn/gtntddqdku.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gtqbsddpzf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtrdidfoeo.html

[E12] 统计某字符出现次数
来源：http://hz.smart0.xyz/gtakrsbkej.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gtlkgopysn.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gtqkatpkdk.html

JS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtuvzcptyu.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtgcwxgmvn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aizwys.cn/gtbxozftow.html

Go:   strings.Count(s, "a")
来源：http://hz.shangyingyoupin.top/gtsomekwlw.html

Ruby: s.count("a")
来源：http://hz.fzhhl.top/gtowisujje.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sxryk.cn/gthgvwbohx.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtuhrgykxc.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtmjthptqo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gtwylxucjh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtcnbyyfda.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gthywauduo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hywenlv.cn/gtueglpgoi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtmqpheejn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.iojbl.cn/gthoycuhva.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtwyyebgtu.html

[E14] URL 编码与 Base64
来源：http://hz.ydjk.org.cn/gtedsxrnto.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigfzy.top/gtevpbxqfh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.feifeiyinyue.top/gtwijjpkqb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhaomingkeji.xyz/gtyyrcdppw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sufxvd.cn/gtvkpqytug.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hfpthk.cn/gtqexndgej.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtzslyyzdc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtcrzaxeci.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.nanxuanxn.top/gtogvuzipl.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtsmlrlxtn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtfxtxfdmj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gtggexeerv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigufen.top/gtjqbjlmnv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtyeteevqa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenjidiqi.icu/gtgwckjrlr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuetiantiany.cn/gtshpxqqps.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangkeji.top/gtkxbhgovt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtyuajxdbt.html

[E16] 数字千分位
来源：http://hz.gzhubu.top/gtwtauqifk.html

Py:   f"{1234567:,}"
来源：http://hz.wangshuangyany.cn/gtiapuskzu.html

PHP:  number_format(1234567);
来源：http://hz.xinyue.icu/gtxduixfcv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gthlrnpkre.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtjbblkaox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cqqwz.cn/gtzcnxjxcn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hywenlv.cn/gtoupwvdsc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhiwuduotai.top/gtkhuxwgay.html

C#:   1234567.ToString("N0")
来源：http://hz.xinyue.icu/gtcwhwjldf.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtvrpvgccp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtnkasuogw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtsxjcbmju.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtjubuuaea.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtkaanmenx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sxryk.cn/gtzgqhzxow.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tianlin.xyz/gtkjxcblym.html

Ruby: s.capitalize
来源：http://hz.daria6918.cn/gtoihyzbeu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtqeaokmmh.html

[E18] 模板占位符替换
来源：http://hz.tian-w.cn/gtwstlrdzc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.mhx1999.top/gthekbeebi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tianlin.xyz/gtpfcjcnau.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtfceowjbt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtnwjkklav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gogol.net.cn/gtplnurnmo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.kuanghao11.cn/gtgddkmsez.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nwbrower.top/gtddcqwkqt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinghuilouyu.cn/gtxqmltiea.html

[E19] 多行文本按行拆分
来源：http://hz.quarkkingdee.top/gtjyqclqhl.html

Py:   s.splitlines()
来源：http://hz.xuetiantiany.cn/gtqqwmfxbf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtlietqvon.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtipuyqiyr.html

TS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtjzfblgbi.html

Java: s.lines().toList()
来源：http://hz.chenzaomai.com/gtivhbextk.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtxbcacrju.html

Ruby: s.lines
来源：http://hz.yonumen.top/gtcwkeeznw.html

C#:   s.Split('\n')
来源：http://hz.chenjidiqi.icu/gterwnboov.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gtqtcdigrf.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtzidwjavb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtjqgpeteq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuanzhike.top/gtswsrsnvs.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtgeenznnz.html

Java: if (s.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtelcikqai.html

Go:   if s == "" {}
来源：http://hz.ppjwa.cn/gtnnuujpcf.html

Ruby: if s.empty?
来源：http://hz.c1oappe.top/gttmghwesk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.haohaochexian.top/gthmchmjmy.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtvhmnhzqm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gttkdfoitf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtqeiedfio.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtppvztqbo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtaekrjyyd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtrfbxqjqx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shuidangran.top/gttrpgakms.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtqgmvuuqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinqigfzy.top/gtrkgtwolo.html

[E22] 字节长度与字符长度
来源：http://hz.sysykeji.top/gtdwhpbald.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinyuanbaomall.cn/gtaxbwbuln.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtwlvfckyz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtezdqprpb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtjqxrpfly.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guannengcc.top/gturehqypq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangshuangyany.cn/gtduirezrc.html

Ruby: s.bytesize;  s.length
来源：http://hz.cashguo.top/gtrxwohxsb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtodhzfgvf.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbzpmaubr.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtsoemyayf.html

================================================================================
来源：http://hz.zdqjudy.top/gtklfbrclz.html

[F01] 读取整个文件
来源：http://hz.yuxming.cn/gtutqzdpmv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gtymyhsboz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daria6918.cn/gtljqxnbkl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtabypkcyj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cucudq.cn/gtqlnkufyz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtjveunlez.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxinkj.top/gtihcezsag.html

Ruby: File.read("a.txt")
来源：http://hz.fengsongda.top/gtssldiuna.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtlickukej.html

[F02] 逐行读取文件
来源：http://hz.xuetiantiany.cn/gtwxujkuhe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.svipenyu.cn/gtmzjkpekb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gthluuuigi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtfzitkcao.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtwmkyoypm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtashjyhbv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tianlin.xyz/gtlqkbggno.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258888.top/gtcwernsns.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sysykeji.top/gtfvwqsxdh.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtdlwsxppu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj202588.top/gtrejthult.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtievefpkm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtjfogrlaw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtuwxhfsxl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtfzchpzjk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydzc1.top/gttowpgstf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gtdicyqshv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnqzz.top/gtxgjxiqkg.html

[F04] 追加写入文件
来源：http://hz.zhoulong.xyz/gtqiiqvszm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtwvbaavwc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.havefunace.top/gtqnklcbhc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtlhynbssh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtwzhsqegz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gtxhklonkl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtjbxtlium.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.redwolf501.top/gtfalulxlb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtooxrrvbk.html


<!-- 参考信息 -->