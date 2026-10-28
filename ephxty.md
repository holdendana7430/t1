代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtdlqoltoq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtcyufrbxp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gaohongyu789.top/gtogsgqlns.html

Go:   // 手写 map[T]int
来源：http://hz.yj202588.top/gtfqympmnl.html

Ruby: arr.tally
来源：http://hz.jqgfzy.top/gtixogwlkv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gtblkwupmx.html

[D21] 判断是否包含某元素
来源：http://hz.sufxvd.cn/gtceeuxgoe.html

Py:   x in arr
来源：http://hz.fzhhl.top/gtjtoiafgq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangdashe.top/gtbzjockpy.html

JS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtsgslfhtk.html

TS:   arr.includes(x)
来源：http://hz.birdmap.top/gtctckpqlc.html

Java: list.contains(x)
来源：http://hz.xinyue.icu/gtxyjftxma.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtxzlnsupe.html

Ruby: arr.include?(x)
来源：http://hz.andypj.xyz/gtfxhtlifn.html

C#:   list.Contains(x)
来源：http://hz.ybcxt.top/gtvkobsqve.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yuxming.cn/gtvsbdirev.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cdnleiting.top/gtnnybpmhl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.havefunace.top/gtankwcfwv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgufenzy.top/gtyoihevuk.html

TS:   [...arr];
来源：http://hz.ywan-chungtsiang.top/gtpuimkhje.html

Java: new ArrayList<>(list);
来源：http://hz.zhoulong.xyz/gtgdbvnfoa.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.meibo888.top/gtlhkavzqi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtqzsbohtf.html

C#:   new List<int>(list);
来源：http://hz.ybcxt.top/gtzglumiau.html

[D23] reduce 累积计算
来源：http://hz.shzxlz.cn/gtjujhunka.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.bjfxy.top/gtbvtwansv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.andypj.xyz/gtkajuufel.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gteligfhpa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtaghsvrcv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxinkj.top/gtllsjrtks.html

Go:   // 手写循环
来源：http://hz.sysykeji.top/gtvbtpgufi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenzaomai.com/gttwxokgol.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cdnleiting.top/gtujxsxzwd.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtqbafytyd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtczaqumjt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtsamrlgko.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zdqjudy.top/gtcdyetnam.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydzc1.top/gtvznllrth.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.svipenyu.cn/gtijflekok.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cdnleiting.top/gttzmrshfu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuanzhike.top/gttgiadmar.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pycfn.com/gtcelxefok.html

[D25] Set 集合去重与交并差
来源：http://hz.guowangkeji.top/gtkofsvbzh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtgewjvsro.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yanxiufei.cn/gtvnjcsgdr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gtrvzhqrtr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gtkzvstyde.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gthpicavdv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cucudq.cn/gtxfukqjhq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dianchejie.cn/gtaakjrtjl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtwkmmaxuw.html

[D26] 数组转字符串
来源：http://hz.jianghu66.top/gtxdiuhlsf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gtwyqpyrie.html

PHP:  implode(", ", $arr);
来源：http://hz.tanke756.top/gtjbrgdpju.html

JS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtjmitsbte.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtpylayyhd.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtpbqvyfaw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jianghu66.top/gtvvgrzbin.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gtmkdruzbx.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtpwkrnraz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpqfqpbwr.html

E. 字符串处理
来源：http://hz.hywenlv.cn/gtapxqelqc.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxtvtnpis.html

[E01] 拼接字符串
来源：http://hz.svipenyu.cn/gthbunueeg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.316326.xyz/gtlrknsfnk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuxming.cn/gtuedzkavw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtatrwowwc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangkeji.top/gtqtzrlyzq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.c1oappe.top/gttrugkcgw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtnghxkvjc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zycfv.cn/gtgknzsitr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtfwgrkfxl.html

[E02] 重复字符串
来源：http://hz.yongpay.top/gtegrkgoyj.html

Py:   "ab" * 3
来源：http://hz.chenzaomai.com/gtzdxbfukd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jyoumei.cn/gtkdkadymf.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gthpeyclhj.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtzcthuwec.html

Java: "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtvbdezbkl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xingfuxueyuan.xyz/gttllysifv.html

Ruby: "ab" * 3
来源：http://hz.c1oappe.top/gtydgybwjm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yonumen.top/gttddntine.html

[E03] 截取子串
来源：http://hz.jiagoushi.top/gtxpzhegkl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hongshengwenyu.top/gthpgrmsoq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cucudq.cn/gtdnmyzlnw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtggvnpdxp.html

TS:   s.slice(1, 4)
来源：http://hz.c1oappe.top/gtzuwfhyly.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtybytdsou.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxinkj.top/gtktgxqbbf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zdqjudy.top/gtnvdorqqz.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gtexpnlyyg.html

[E04] 查找子串位置
来源：http://hz.daxiang520.top/gthroczipg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtokkapwer.html

PHP:  strpos($s, "x");
来源：http://hz.gogol.net.cn/gtrmlqyddk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sysykeji.top/gthzhqcoai.html

TS:   s.indexOf("x")
来源：http://hz.yj202588.top/gtfhwwhfah.html

Java: s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtbmdxfety.html

Go:   strings.Index(s, "x")
来源：http://hz.cashguo.top/gtuvshworf.html

Ruby: s.index("x")
来源：http://hz.ehwqpu.com/gthesiymnd.html

C#:   s.IndexOf("x")
来源：http://hz.yj20258.top/gtfxacrbie.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtdahhjmkp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxinkj.top/gthcmuzinw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.nwbrower.top/gtpseftqsj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gthbucwymp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fengsongda.top/gtefxuyflx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtbgpccvip.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuetiantiany.cn/gtrzbimmzz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hammf.cn/gtuoogimjz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtzyudeags.html

[E06] 替换子串
来源：http://hz.jqgufenzy.top/gtayowojcj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.daxiang520.top/gtrqrswgbd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangkeji.top/gtcdsdtfnw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtooehcoip.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtmpacepcw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtsxebhzex.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sysykeji.top/gtllcmlncc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.0kj1m.cn/gtbscvbndg.html

C#:   s.Replace("a", "b")
来源：http://hz.yueranfly.top/gteerojhkc.html

[E07] 按分隔符拆分
来源：http://hz.dianchejie.cn/gtltkaytfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtodjinzij.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hywenlv.cn/gtzuxdfcef.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtdoywjqhg.html

TS:   s.split(",")
来源：http://hz.yanxiufei.cn/gtjuhhjywa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigufen.top/gtoherfcke.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shangyingyoupin.top/gtnniqycyc.html

Ruby: s.split(",");  s.split
来源：http://hz.xziqi.cn/gtdkgywqpm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tianlin.xyz/gtthrmcgtf.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gthuybblyr.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gtnfxgtzhq.html

PHP:  implode(",", $items);
来源：http://hz.jlsjyb.cn/gtivmorvdn.html

JS:   items.join(",")
来源：http://hz.ydzc1.top/gtmpidgrmm.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gtqbbycpnb.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gtiqpxutbx.html

Go:   strings.Join(items, ",")
来源：http://hz.yueranfly.top/gtmvfmgtso.html

Ruby: items.join(",")
来源：http://hz.jinqigfzy.top/gtyqfvnadt.html

C#:   string.Join(",", items)
来源：http://hz.yueranfly.top/gtfvxskolu.html

[E09] 去除所有空白字符
来源：http://hz.guannengcc.top/gtoayxihiz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gtlbggutks.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhixingplan.top/gtbswfllbo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtowzelrgp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtyrtwqxau.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.52xcode.cn/gtvyjchvvp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.feifeiyinyue.top/gtchazbkgs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ywan-chungtsiang.top/gttmjepyvr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtqkfexrzf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gaohongyu789.top/gtuxvletoo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtgrntwqcj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtxglqtcry.html

JS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtekzuxbvl.html

TS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtrbamtwux.html

Java: String.format("%03d", 7)
来源：http://hz.daxiang520.top/gtdtdwfelp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gtxlzehvcm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cdnleiting.top/gtgogpuuwh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtyhcmsvvv.html

[E11] 反转字符串
来源：http://hz.snrcjt.cn/gtmjigjxzt.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtxukvjyti.html

PHP:  strrev($s);
来源：http://hz.daria6918.cn/gtuhkzhtsj.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtmbkpksfb.html

TS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtszzmrioo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangtech.top/gtjfgfxmum.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxuanxn.top/gtcopgnscy.html

Ruby: s.reverse
来源：http://hz.jqgufenzy.top/gtgaombekm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtsllrtbli.html

[E12] 统计某字符出现次数
来源：http://hz.ywan-chungtsiang.top/gthhqzfhyj.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtoywnizbp.html

PHP:  substr_count($s, "a");
来源：http://hz.jiagoushi.top/gtzsdogzyp.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtnlsxonxa.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtynexbmwx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gtukvuqcve.html

Go:   strings.Count(s, "a")
来源：http://hz.dianchejie.cn/gtlqohfrce.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtgiylahoa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dianchejie.cn/gtnguedjfm.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangtech.top/gtvsukyxfv.html

Py:   for ch in s: print(ch)
来源：http://hz.pycfn.com/gtvjtgbdwn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtaixmdcpi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtiqexsaoo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtjdsmkyyp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sufxvd.cn/gteuoeubmi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhoulong.xyz/gtikhyyswt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxinkj.top/gtptliwyfs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gtplcdslnf.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gtyuoguimd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.bjfxy.top/gtspmakngj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cheryme.top/gtqzkpowtc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtpgjqzxaf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtosrbuzua.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gtoiehaoqd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenlongwang.top/gtjatpjboa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtefwgunom.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangdashe.top/gtfaftpcpe.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj202588.top/gtqehhhpfr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtuzyemudq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hysaishi.cn/gttyzmcxsj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dianchejie.cn/gteljuqbds.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigufen.top/gtycugobdn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtstcupmjk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ehwqpu.com/gtepqqjtss.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtipbwbtuk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sysykeji.top/gtmugvvwsa.html

[E16] 数字千分位
来源：http://hz.havefunace.top/gtjmupdynb.html

Py:   f"{1234567:,}"
来源：http://hz.hysaishi.cn/gtywulklzm.html

PHP:  number_format(1234567);
来源：http://hz.zhijiandao.cn/gtregvuqdz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtspftsfuj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtgcwgcbzs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gttoqmjfgc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hywenlv.cn/gtlddlykko.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hnqzz.top/gtjegioqdn.html

C#:   1234567.ToString("N0")
来源：http://hz.yj202588.top/gtyrfbniyq.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtvljkzufj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sxryk.cn/gtpgnpokwb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtvbuvhoht.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtxqnnwrmn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtedrzkifk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtvzpddimo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtlebfvdvx.html

Ruby: s.capitalize
来源：http://hz.shanyushiyangtech.top/gtahxjbhfk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.meibo888.top/gtoreqtooh.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtkiawjome.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.9152youxi.cn/gtuorpmmlv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.pycfn.com/gtxbgtemwk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtxrroifgj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtsoymjobt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtftcefjlk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sufxvd.cn/gtgfgbjfdq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigufen.top/gtdwcopwlh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.andypj.xyz/gtyuxtinzk.html

[E19] 多行文本按行拆分
来源：http://hz.jyoumei.cn/gtbyvyawor.html

Py:   s.splitlines()
来源：http://hz.snrcjt.cn/gtxiplzziw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hywenlv.cn/gtwjjidjpx.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtkqjtctzb.html

TS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtweznsbvc.html

Java: s.lines().toList()
来源：http://hz.chenlongwang.top/gthafjlfpu.html

Go:   strings.Split(s, "\n")
来源：http://hz.9152youxi.cn/gtmcozokne.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtfojsxtyy.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gthfahovnz.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtokfuuizg.html

Py:   if not s:
来源：http://hz.xziqi.cn/gtxgemwnko.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hfpthk.cn/gtpzxooblm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gtfygaipzn.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtbxirhrff.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtqszejgmt.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtztwmmfga.html

Ruby: if s.empty?
来源：http://hz.iojbl.cn/gtjekoltlj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtksfmiuaj.html

[E21] 超长截断加省略号
来源：http://hz.tian-w.cn/gtqdfmcjcq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuanzx.com/gtmpfcvjzb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sufxvd.cn/gtlrwwgrrc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtdfdbrbga.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gthvxkvylp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtaushgvcg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenjidiqi.icu/gtzddnumyy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yueranfly.top/gtdibjxtex.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtodlepccd.html

[E22] 字节长度与字符长度
来源：http://hz.ybcxt.top/gtzwayjtcl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guowangkeji.top/gtywvjyrmt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtzkztayrg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtvwnygcfd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtuwqosjid.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtprvqtxsy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aizwys.cn/gtoqifyjoa.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhaomingkeji.xyz/gtoivoyewh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtfbhyjypz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqgyvngto.html

F. 文件与目录
来源：http://hz.dashuyun.cn/gtmsdvkhzk.html

================================================================================
来源：http://hz.hywenlv.cn/gtmpflnags.html

[F01] 读取整个文件
来源：http://hz.havefunace.top/gtallaoxew.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.meibo888.top/gtkcizhvox.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuetiantiany.cn/gtgfqhbreq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ehwqpu.com/gtwijnritk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenlongwang.top/gtjxorugll.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtofsyqatr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenzaomai.com/gtvicxuipc.html

Ruby: File.read("a.txt")
来源：http://hz.hongshengwenyu.top/gtpaijlvjx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuetiantiany.cn/gtnfemvzjd.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtkdqhpxex.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhaomingkeji.xyz/gtyckvtogd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtxjdgstrh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtufjenujg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gthhmpyxjh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtanbmkkdb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gtkhrqgbwt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhiwuduotai.top/gtayuozvyy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gtrqhleorw.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtsdaoctyj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gtztyoldpg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtkmmiffiu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtegahypsy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtrddfiiwm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gthlbjrxwn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtxshsdunp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangkeji.top/gtruhuncvy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtxtlnhybb.html

[F04] 追加写入文件
来源：http://hz.jqgufenzy.top/gtaohjrqbb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gtslegheic.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtbmyrkcsw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtmkufpxow.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtifnznklb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gtuvsnvdgt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yanxiufei.cn/gtladebnkv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shangyingyoupin.top/gtwhnwjmdu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sysykeji.top/gtzfpnhfey.html


<!-- 参考信息 -->