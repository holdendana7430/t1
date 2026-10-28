代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hywenlv.cn/gtdxcyepuw.html

[D20] 统计每个元素出现次数
来源：http://hz.yuxming.cn/gtmgtkkhny.html

Py:   Counter(arr)
来源：http://hz.zhoulong.xyz/gteinkokru.html

PHP:  array_count_values($arr);
来源：http://hz.zdqjudy.top/gtoilsazwn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtptzjacqr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gteemzawio.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgfzy.top/gtntdmrycc.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gtfmzegpfr.html

Ruby: arr.tally
来源：http://hz.mhx1999.top/gtinnzutjm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtfpfdmrnf.html

[D21] 判断是否包含某元素
来源：http://hz.tianlin.xyz/gtydurapsi.html

Py:   x in arr
来源：http://hz.mhx1999.top/gtzxxdarge.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ywan-chungtsiang.top/gtpohjiiag.html

JS:   arr.includes(x)
来源：http://hz.yj202588.top/gtcftvzkry.html

TS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtcjsaccad.html

Java: list.contains(x)
来源：http://hz.jinqigufen.top/gtwpjrqvne.html

Go:   slices.Contains(arr, x)
来源：http://hz.xinyue.icu/gtdvomwzam.html

Ruby: arr.include?(x)
来源：http://hz.iojbl.cn/gtendmtezd.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtphlwshiz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ivvv.top/gtfqkrujfd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhoulong.xyz/gtqckhgpeq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangtech.top/gtfosxchch.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jianghu66.top/gtvlmktaao.html

TS:   [...arr];
来源：http://hz.yvedp.cn/gtmklmjsct.html

Java: new ArrayList<>(list);
来源：http://hz.cashguo.top/gtrvlfpxnh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ywan-chungtsiang.top/gtscgaovnl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gotoacloud.top/gtzgnpepdk.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gtqhannrmr.html

[D23] reduce 累积计算
来源：http://hz.sweek.top/gtntvnwzqa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.snrcjt.cn/gtglthridq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinghuilouyu.cn/gtgzvjbqbk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtjhzcdcaa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtdtvhjxjn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ywan-chungtsiang.top/gtsekompxt.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtufgkxlye.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yvedp.cn/gtnljpmsks.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xingfuxueyuan.xyz/gtxcaxkimd.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtvxdnkuim.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.haohaochexian.top/gtlagfedyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xingfuxueyuan.xyz/gtqzwlbogk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cdnleiting.top/gtvpxjcvqi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.mhx1999.top/gtlcfnlyuk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cheryme.top/gtionnlrwz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.andypj.xyz/gtbcglapkz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gtocxrigfz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ywan-chungtsiang.top/gtfarvyzzc.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtobwyhobz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cheryme.top/gtojsrfshw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ppjwa.cn/gtrtskwvxm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tianlin.xyz/gtznqciyxm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtjidgmokb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtnamobhrh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nwbrower.top/gteuqfhrlu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shzxlz.cn/gtrokcackh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtbiacnjsc.html

[D26] 数组转字符串
来源：http://hz.hywenlv.cn/gtfgjgqfbb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.quarkkingdee.top/gtksqcobpi.html

PHP:  implode(", ", $arr);
来源：http://hz.gogol.net.cn/gtrynnqfak.html

JS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtbbpnxttk.html

TS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtufjxcxbv.html

Java: String.join(", ", list)
来源：http://hz.ybcxt.top/gtlsobidnu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.pycfn.com/gtkzdqciea.html

Ruby: arr.join(", ")
来源：http://hz.cucudq.cn/gtptqhkkpk.html

C#:   string.Join(", ", list)
来源：http://hz.jinyuanbaomall.cn/gtblyvtdeh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsmquuieg.html

E. 字符串处理
来源：http://hz.nanxinkj.top/gtfimkecdd.html

================================================================================
来源：http://hz.pycfn.com/gthioftbno.html

[E01] 拼接字符串
来源：http://hz.dashuyun.cn/gtgtpacmps.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258888.top/gtzkihzofu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hfpthk.cn/gtwzfwsafv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtggcqtojn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtpsfjgrlb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xingfuxueyuan.xyz/gtocytppfa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.bjfxy.top/gtmxjnsoho.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxinkj.top/gtaowtshoy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtkccjouoq.html

[E02] 重复字符串
来源：http://hz.vqdsnc.cn/gtxyanaewa.html

Py:   "ab" * 3
来源：http://hz.jianghu66.top/gtknuxewcd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtgcjjwwfd.html

JS:   "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtwabtwxif.html

TS:   "ab".repeat(3)
来源：http://hz.daria6918.cn/gtrtfiioek.html

Java: "ab".repeat(3)
来源：http://hz.fzhhl.top/gtxegmunef.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daria6918.cn/gtsosgjfli.html

Ruby: "ab" * 3
来源：http://hz.redwolf501.top/gtqyhtkmmd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shangyingyoupin.top/gtahgtvlru.html

[E03] 截取子串
来源：http://hz.fengsongda.top/gtltfumlsh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtxmpowgwx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtmwpptdif.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fengsongda.top/gtdgvzwozn.html

TS:   s.slice(1, 4)
来源：http://hz.jyoumei.cn/gtqmtvmkfi.html

Java: s.substring(1, 4)
来源：http://hz.hammf.cn/gttkcekqsd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fengsongda.top/gtqktvfwcq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gogol.net.cn/gtfswoznre.html

C#:   s.Substring(1, 3)
来源：http://hz.cqqwz.cn/gttausalbk.html

[E04] 查找子串位置
来源：http://hz.havefunace.top/gtvdbkvlfw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hnxiangtu.top/gtrjtcqjle.html

PHP:  strpos($s, "x");
来源：http://hz.hfpthk.cn/gtelhzglym.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangshuangyany.cn/gtfmhrgfjs.html

TS:   s.indexOf("x")
来源：http://hz.yongpay.top/gtlecjqcxm.html

Java: s.indexOf("x")
来源：http://hz.andypj.xyz/gtpkjtrrny.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gtvnbqcgws.html

Ruby: s.index("x")
来源：http://hz.aibaodan.cn/gtploivixa.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gtkoyrskya.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtzbxvxzrf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtwpftqwnr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenzaomai.com/gtqvveorry.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtvbvsmwzc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dashuyun.cn/gtonlaeawf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ywan-chungtsiang.top/gtupkmmzll.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtinblhmok.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtymaurmam.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gzhubu.top/gtcqdsacgj.html

[E06] 替换子串
来源：http://hz.jqgufenzy.top/gtmzmbwzlm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.havefunace.top/gtlkdqjgdf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtqzabrxmr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtxhyzednh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtdropgfoi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtjytjyacs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtigwbdlff.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yanxiufei.cn/gtpkyssczi.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtdktwfugw.html

[E07] 按分隔符拆分
来源：http://hz.yj202588.top/gtdqsmujhe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gotoacloud.top/gtcnukvmwv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinghuilouyu.cn/gtitepzvbq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.c1oappe.top/gtazwfpiog.html

TS:   s.split(",")
来源：http://hz.zhiwuduotai.top/gtnbjotouc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenjidiqi.icu/gtticvikra.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj202588.top/gtiuwepvef.html

Ruby: s.split(",");  s.split
来源：http://hz.zhoulong.xyz/gtkymdpuoz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xuanzx.com/gtacchquye.html

[E08] 数组按分隔符合并
来源：http://hz.jqgfzy.top/gtftobzvcj.html

Py:   ",".join(items)
来源：http://hz.svipenyu.cn/gtgompaext.html

PHP:  implode(",", $items);
来源：http://hz.tianlin.xyz/gtpawumwmk.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtfmhqztad.html

TS:   items.join(",")
来源：http://hz.dashuyun.cn/gtrqnprzof.html

Java: String.join(",", items)
来源：http://hz.gzhubu.top/gtqjorutgj.html

Go:   strings.Join(items, ",")
来源：http://hz.xylfe.cn/gtfsiicegt.html

Ruby: items.join(",")
来源：http://hz.jyoumei.cn/gtwbbloush.html

C#:   string.Join(",", items)
来源：http://hz.tanke756.top/gtssexwxpg.html

[E09] 去除所有空白字符
来源：http://hz.dianchejie.cn/gthznoysxi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ywan-chungtsiang.top/gtfnbnkrmj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtkhnuhtqw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtjvthyqyu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtrhfjkufn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ybcxt.top/gtohudjlfx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.52xcode.cn/gtrjimmppg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yueranfly.top/gtnqnikpip.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuetiantiany.cn/gtqjvxnmtt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.quarkkingdee.top/gtsbqzztix.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.andypj.xyz/gtqvnqergg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigfzy.top/gtrgugayqd.html

JS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtjylstusg.html

TS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gttpdhxxvj.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtctkduesq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtdncputaa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gtsrnolxhi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gthsyiqaie.html

[E11] 反转字符串
来源：http://hz.shuidangran.top/gtyczohjcb.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gtlpqliqjl.html

PHP:  strrev($s);
来源：http://hz.cucudq.cn/gtapcbflia.html

JS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtmtahmfoo.html

TS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtwtvmfape.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aibaodan.cn/gtktuvkyvh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.smart0.xyz/gtjwxgnckh.html

Ruby: s.reverse
来源：http://hz.yj20258.top/gtgveqqxjc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtofidnltc.html

[E12] 统计某字符出现次数
来源：http://hz.iojbl.cn/gtxcohpyvv.html

Py:   s.count("a")
来源：http://hz.yonumen.top/gtcwwvoujq.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtwawhhjbp.html

JS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gtfcnoxzxr.html

TS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtgohyyzsm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hywenlv.cn/gtagrdrkrw.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtqlzimbtb.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtmwyzduhw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gtfkbibdju.html

[E13] 逐字符遍历
来源：http://hz.jianghu66.top/gtycrjgmce.html

Py:   for ch in s: print(ch)
来源：http://hz.chenjidiqi.icu/gtchplykog.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydjk.org.cn/gtmgoiacbc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtllxxwvvm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtgmiuhype.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gttffexcxa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yvedp.cn/gtceacviiv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sxryk.cn/gttwuavahi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtsoilimzn.html

[E14] URL 编码与 Base64
来源：http://hz.hnxiangtu.top/gtilkqiker.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gtgzmsrkvr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shuidangran.top/gtrqhvnpsk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gtmxyyavqu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuetiantiany.cn/gtimzluuia.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuanzx.com/gtbkadessv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xingfuxueyuan.xyz/gtqkfxltsj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hysaishi.cn/gtupmuszad.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtvmswcwna.html

[E15] HTML 转义 / 反转义
来源：http://hz.9152youxi.cn/gtkhgovwzj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenzaomai.com/gtzyacmeqc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtcevxjhsr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtexdppglu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daxiang520.top/gtoqshgmql.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gteekqebpw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.316326.xyz/gtcptoccde.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jiagoushi.top/gtllzuigkr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hywenlv.cn/gtljgmjfmo.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gtgzlldcey.html

Py:   f"{1234567:,}"
来源：http://hz.sufxvd.cn/gtgfkkhbrj.html

PHP:  number_format(1234567);
来源：http://hz.ydjk.org.cn/gtgfwmwfum.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtvqkwtivn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtnynrhvpn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258888.top/gtudbcwles.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinghuilouyu.cn/gtesezpamv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtjkikswdt.html

C#:   1234567.ToString("N0")
来源：http://hz.zdqjudy.top/gtgxevgxcp.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtawassuge.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ehwqpu.com/gtlngufzoo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtaihahria.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gtskttfbdb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtgwlnxbez.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tianlin.xyz/gtnotsopmr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tian-w.cn/gtiqykkcch.html

Ruby: s.capitalize
来源：http://hz.xziqi.cn/gthgiipqnc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtmlsbdidl.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gttpqsxepo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangdashe.top/gtkwbtnlwu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhiwuduotai.top/gtoxcrvfoi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtaxbzdbnb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gtwajrqdqc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258.top/gttfhczqwt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gtzplharnw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.mhx1999.top/gtryratwwf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gttogiyquf.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtlnmdqjkx.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtlofbauwt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtdwawemtk.html

JS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtphcprkyi.html

TS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtsyjvqlhm.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtthbogipl.html

Go:   strings.Split(s, "\n")
来源：http://hz.vqdsnc.cn/gtxxfvncgp.html

Ruby: s.lines
来源：http://hz.hysaishi.cn/gtpsoqoyvv.html

C#:   s.Split('\n')
来源：http://hz.mhx1999.top/gtmkgbfodv.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtemygcpry.html

Py:   if not s:
来源：http://hz.pycfn.com/gtbhgptbkj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtdtgvzhbm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtnrdvwjuz.html

TS:   if (s === "") {}
来源：http://hz.jinqigufen.top/gtmjhtiboj.html

Java: if (s.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtuarxkbym.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gtvdvomnnh.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtoldonmbn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fzhhl.top/gtiqbpqkze.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gtqwgtlliq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxinkj.top/gtcydnhpsr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ydjk.org.cn/gtncgbtiju.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtsuxgapml.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtuvdfthmy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gttmjcdixy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtqjzyzonx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydzc1.top/gtklvuavnr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gtmgjgejrr.html

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtdxmtgeld.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gotoacloud.top/gthqkfqpng.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtvmrhkfdq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtwdwmjjsf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtjqccagzj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.feifeiyinyue.top/gtwnaglyvx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtdfwkzpry.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtvwldjbos.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtvelwmmyo.html

================================================================================
来源：http://hz.wangdashe.top/gtqawllcpu.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtqezgyuqt.html

================================================================================
来源：http://hz.fengsongda.top/gtwdozerzp.html

[F01] 读取整个文件
来源：http://hz.tian-w.cn/gthgvtztqh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.havefunace.top/gtujexfkyc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cucudq.cn/gtvvpixlre.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xylfe.cn/gtifklljcw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtzuvkyero.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gthxjrmbwi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtdfvcywnw.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gtfpgvefye.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtyyhbdcym.html

[F02] 逐行读取文件
来源：http://hz.iojbl.cn/gtajrqiseh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtgywwnnlg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cheryme.top/gtklntjqhr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtjazxppru.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtkajsqqmx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtebuhmrur.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgufenzy.top/gtgagwwhut.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fengsongda.top/gtexltwvjm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jlsjyb.cn/gtotkwirhp.html

[F03] 写入文件（覆盖）
来源：http://hz.yvedp.cn/gtapipdvjk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cheryme.top/gtqgymnnfm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtbxzeqnhm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtgjdyckxf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtayxdxhmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.haohaochexian.top/gtamvaxhsd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtqrubwdie.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gtegwshwkl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sxryk.cn/gtqvybclqp.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gtarppsrre.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gaohongyu789.top/gtvpcvcerd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhaomingkeji.xyz/gtzfkdbmna.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtjfjwdldc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtnlvkqhej.html


<!-- 参考信息 -->