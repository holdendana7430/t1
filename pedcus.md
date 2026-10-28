代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangdashe.top/gtljrloahs.html

C#:   list.Sum();  list.Average()
来源：http://hz.zdqjudy.top/gtdjuvhscy.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtvuqxjtts.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtxkhnjcts.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gtthjrrjuh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtojnngpoq.html

TS:   Math.max(...arr);
来源：http://hz.52xcode.cn/gtvgaqmuou.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gtfwqsbwoq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yvedp.cn/gtwqkkeppo.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gtklqrzcpo.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtakjybjtb.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gtxyporirz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daxiang520.top/gtgomrvoaq.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtvgducxai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jyoumei.cn/gtvshfevcm.html

TS:   nested.flat();
来源：http://hz.chenlongwang.top/gtkkcylbuy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aibaodan.cn/gtvrotvkth.html

Go:   // 手写双层循环
来源：http://hz.chenzaomai.com/gtmzkezxya.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtzhwfurix.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.svipenyu.cn/gtlkvprspg.html

[D19] 按字段分组
来源：http://hz.ivvv.top/gtxnvzrepp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cucudq.cn/gtdrimnssd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gzhubu.top/gttqyfvgph.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.kuanghao11.cn/gtdrowcpxw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yvedp.cn/gtdyjegexs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.vqdsnc.cn/gthwkuvtke.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtbthzsnuz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtcbqiluby.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gtkciqhtmu.html

[D20] 统计每个元素出现次数
来源：http://hz.xinyue.icu/gtvrukbnan.html

Py:   Counter(arr)
来源：http://hz.zhongyouzk.top/gtwjqnkwws.html

PHP:  array_count_values($arr);
来源：http://hz.zhongyouzk.top/gtrhieqmhs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtwsaxvfwb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtiuswzczq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtsvovctkr.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigfzy.top/gtxpctnoms.html

Ruby: arr.tally
来源：http://hz.hnqzz.top/gtzhmqhpsk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shangyingyoupin.top/gtjmtxtkvs.html

[D21] 判断是否包含某元素
来源：http://hz.9152youxi.cn/gtavbjywje.html

Py:   x in arr
来源：http://hz.cheryme.top/gtemseqrxw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gttnftfmnl.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtqhqlcyqg.html

TS:   arr.includes(x)
来源：http://hz.jlsjyb.cn/gtsivegkle.html

Java: list.contains(x)
来源：http://hz.guannengcc.top/gtwaaqdwxe.html

Go:   slices.Contains(arr, x)
来源：http://hz.hysaishi.cn/gtmnodleai.html

Ruby: arr.include?(x)
来源：http://hz.jinyuanbaomall.cn/gtnbutmbgc.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtxlrtvxqi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gthzzfynsu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangkeji.top/gtyorestwk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ivvv.top/gtxpxcdmmv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenzaomai.com/gtbqkmzmrl.html

TS:   [...arr];
来源：http://hz.dashuyun.cn/gthmgmiuvm.html

Java: new ArrayList<>(list);
来源：http://hz.shangyingyoupin.top/gtoeufnwru.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yongpay.top/gtjdhwbkad.html

Ruby: arr.dup;  arr.clone
来源：http://hz.haohaochexian.top/gthpkepnbv.html

C#:   new List<int>(list);
来源：http://hz.hongshengwenyu.top/gtbculxjuk.html

[D23] reduce 累积计算
来源：http://hz.guannengcc.top/gtqftxtdwa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gthfepdibk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ivvv.top/gtfcoxowuc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gteqmyfefc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtutrdbhet.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pycfn.com/gtxjmnipbh.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtbycwjwnz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gtjmlujnht.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258888.top/gtecqgkopg.html

[D24] 字典 / Map 基本操作
来源：http://hz.sxryk.cn/gtheswuoyn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gtiujawqar.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhixingplan.top/gtpnfolppm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangtech.top/gthovmckfy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shzxlz.cn/gtajxgpzqm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gtwxusyeor.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenjidiqi.icu/gtrwjkdgbj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hammf.cn/gthfrqvkgt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnxiangtu.top/gtlcrdcejo.html

[D25] Set 集合去重与交并差
来源：http://hz.jyoumei.cn/gtmlgqjvro.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yvedp.cn/gtcecgosin.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtdjrsjhfj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuxming.cn/gtloqwgdhi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.c1oappe.top/gtlcdkwvkn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.meibo888.top/gtntjtfnrr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jyoumei.cn/gtubmknitg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sxryk.cn/gtzdynslsi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhoulong.xyz/gthcaeziyj.html

[D26] 数组转字符串
来源：http://hz.zhongyouzk.top/gtspkqgunj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxinkj.top/gtcwljdbwc.html

PHP:  implode(", ", $arr);
来源：http://hz.sysykeji.top/gtimxlfikf.html

JS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtjpawamgt.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtihideqto.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtwlcnkaxn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nwbrower.top/gthhzvjolx.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtmtafinev.html

C#:   string.Join(", ", list)
来源：http://hz.yangfankeji.com/gtzhnadkuz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtcjcitrzq.html

E. 字符串处理
来源：http://hz.bjfxy.top/gtxokwyqbb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqwrtvpvb.html

[E01] 拼接字符串
来源：http://hz.cashguo.top/gtwxekpnlp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cqqwz.cn/gtbyxabiwv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cucudq.cn/gtusqmtcdb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtbcebhrgc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtuqumqahj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jianghu66.top/gtavdoiyxf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtblkbnnxs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yanxiufei.cn/gtwjgzwymy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sufxvd.cn/gtqgmbmgki.html

[E02] 重复字符串
来源：http://hz.ivvv.top/gtearqchve.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtziejsxcq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtoalcehjq.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtzrqnlpgc.html

TS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtfquvhacn.html

Java: "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtutrazcrp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.haohaochexian.top/gtytkpamih.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtujaqiupf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zdqjudy.top/gtiolsftbk.html

[E03] 截取子串
来源：http://hz.aizwys.cn/gtsoejmnwy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.snrcjt.cn/gtskktgwqd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gtszjytzca.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tanke756.top/gtsaezvyib.html

TS:   s.slice(1, 4)
来源：http://hz.daria6918.cn/gtppoaroxv.html

Java: s.substring(1, 4)
来源：http://hz.pycfn.com/gtxvsuwpeb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gaohongyu789.top/gtlznjynhp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtgbiemfwc.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgfzy.top/gtkqxjpwdp.html

[E04] 查找子串位置
来源：http://hz.sxryk.cn/gtbdqfxkxz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yanxiufei.cn/gthguaszru.html

PHP:  strpos($s, "x");
来源：http://hz.fengsongda.top/gtcshmfjzp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtyfpqhmsz.html

TS:   s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtcgnpumue.html

Java: s.indexOf("x")
来源：http://hz.cdnleiting.top/gtctovifnm.html

Go:   strings.Index(s, "x")
来源：http://hz.daria6918.cn/gtgsmlpypn.html

Ruby: s.index("x")
来源：http://hz.guannengcc.top/gtxohitlsl.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangtech.top/gtkqbpcxxt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.fzhhl.top/gtwweryavl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ywan-chungtsiang.top/gtfxybdpiu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.meibo888.top/gtssdnbjjh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtaemwyhkd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hfpthk.cn/gtntgrlcie.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtnyqeagdz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gzhubu.top/gtfanlyaft.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gtskrgxxbh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydzc1.top/gtuhpqdwon.html

[E06] 替换子串
来源：http://hz.iojbl.cn/gtcgzglpjb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ybcxt.top/gtnfrdzbse.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.iojbl.cn/gtgkzeizfb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtxeghkrzx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtnumjvlqg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtzujpzzco.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xingfuxueyuan.xyz/gttfspxvwt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hfpthk.cn/gtjvfhcakf.html

C#:   s.Replace("a", "b")
来源：http://hz.cucudq.cn/gtymlslini.html

[E07] 按分隔符拆分
来源：http://hz.cheryme.top/gtscnctpsn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zycfv.cn/gtbokqnmbz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jlsjyb.cn/gtcenbhyua.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.pycfn.com/gtqgwsgkqn.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtvgpsexuk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ywan-chungtsiang.top/gtgqcxzszb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhiwuduotai.top/gtdpcusful.html

Ruby: s.split(",");  s.split
来源：http://hz.sweek.top/gthlwwuskl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhijiandao.cn/gtldznmhhy.html

[E08] 数组按分隔符合并
来源：http://hz.zhiwuduotai.top/gttpzeiadr.html

Py:   ",".join(items)
来源：http://hz.jlsjyb.cn/gtzlgpgxvn.html

PHP:  implode(",", $items);
来源：http://hz.meibo888.top/gtickcijzz.html

JS:   items.join(",")
来源：http://hz.andypj.xyz/gtrdyvoiut.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtxibrzbud.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtelqlrkjz.html

Go:   strings.Join(items, ",")
来源：http://hz.iojbl.cn/gtcftlwhjx.html

Ruby: items.join(",")
来源：http://hz.dianchejie.cn/gtimktbdam.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtsqkqsfyo.html

[E09] 去除所有空白字符
来源：http://hz.zhiwuduotai.top/gtmowdfier.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gtzkbsaaom.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtheggnrhy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtvjmuqcqa.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gogol.net.cn/gtebmxnete.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yonumen.top/gtkujjkdlq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gogol.net.cn/gtpewuzbet.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xylfe.cn/gtvamcylvf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hfpthk.cn/gtfanmjxwg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtwlwdtzdi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhiwuduotai.top/gtlzoamolt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhixingplan.top/gtrcsqshuy.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenlongwang.top/gtgvovarre.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtmqzgnqno.html

Java: String.format("%03d", 7)
来源：http://hz.yuanzhike.top/gthrgihbza.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jianghu66.top/gtorxtuiog.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dashuyun.cn/gtrzzgswub.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.9152youxi.cn/gtdhdgpoed.html

[E11] 反转字符串
来源：http://hz.gotoacloud.top/gtqsnmretd.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtpknbtrqn.html

PHP:  strrev($s);
来源：http://hz.smart0.xyz/gtvrjxlvzz.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtrywxhduz.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtwecpiujv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gttaqebfrm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gtybzhrpys.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtikrlwkcw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtiyajzdoc.html

[E12] 统计某字符出现次数
来源：http://hz.ywan-chungtsiang.top/gtuapktumj.html

Py:   s.count("a")
来源：http://hz.daxiang520.top/gtwafdqkzh.html

PHP:  substr_count($s, "a");
来源：http://hz.pengpengdd.cyou/gtqbdfbtly.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtwsbrdfkd.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtvmuxyckl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zycfv.cn/gteokkqyqk.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtcxgswaye.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtayroibfa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gtvgmkcccf.html

[E13] 逐字符遍历
来源：http://hz.jianghu66.top/gtzhswioen.html

Py:   for ch in s: print(ch)
来源：http://hz.ybcxt.top/gtdbaiwiix.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgfzy.top/gtwbyxkryh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtgljbvihx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.c1oappe.top/gtzsdngebx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinghuilouyu.cn/gtfvusaugy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinghuilouyu.cn/gtyqezzrmw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hysaishi.cn/gtmntjbisk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtlkxuaqzb.html

[E14] URL 编码与 Base64
来源：http://hz.xylfe.cn/gtdtzigrpo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jianghu66.top/gtgplfuwpg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pengpengdd.cyou/gtlauowmnb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.smart0.xyz/gtqeskvger.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxinkj.top/gtpjgvspan.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gtkhgqinpz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pengpengdd.cyou/gtrzqatvik.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.52xcode.cn/gtywvaxiat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ehwqpu.com/gtqoiosxgm.html

[E15] HTML 转义 / 反转义
来源：http://hz.tianlin.xyz/gtfhxytaih.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jyoumei.cn/gterdmxerr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtjpgghxbw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.0kj1m.cn/gtvhthmfgi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tanke756.top/gtqsdhkdoa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fengsongda.top/gtbkvuemkb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtqfabmahy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtdvxaqfvo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtsokyczvv.html

[E16] 数字千分位
来源：http://hz.smart0.xyz/gtlyjcmbga.html

Py:   f"{1234567:,}"
来源：http://hz.zhixingplan.top/gtqewhkhmd.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtmhffgxuz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gteihfgtwe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtplgcbxib.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhiwuduotai.top/gtdfxcxucm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fzhhl.top/gttxvutavb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yueranfly.top/gthsubymnm.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtmkefwxwl.html

[E17] 首字母大写
来源：http://hz.xylfe.cn/gttwmcwtii.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtrmofrroh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sysykeji.top/gtfjirreea.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zycfv.cn/gtmwoabxnx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtwlgfhwog.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gtpuaiokup.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gtuissrwag.html

Ruby: s.capitalize
来源：http://hz.vqdsnc.cn/gtbohtrpne.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xingfuxueyuan.xyz/gtsjwdddzj.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtmksfesli.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cheryme.top/gtnlcmkuue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gtaesdxygg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtfaybzsvp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtdmvgwzea.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ehwqpu.com/gtpevbmvje.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gtnpipwyfs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fengsongda.top/gtotlqkasz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtlajzlxlr.html

[E19] 多行文本按行拆分
来源：http://hz.aibaodan.cn/gtdiulubfa.html

Py:   s.splitlines()
来源：http://hz.jqgufenzy.top/gtfavzvakk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtpmwfnsbm.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtrlfnvijt.html

TS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtebatjrse.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gtqwikwide.html

Go:   strings.Split(s, "\n")
来源：http://hz.birdmap.top/gtygccpkcg.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtxftycfgg.html

C#:   s.Split('\n')
来源：http://hz.cashguo.top/gteodsdljl.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtucfpxltq.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtuwxnhlas.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.wangshuangyany.cn/gtmlzywthn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.smart0.xyz/gtlsnojcbg.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtmmmajean.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtogfodswc.html

Go:   if s == "" {}
来源：http://hz.sufxvd.cn/gtfzjvwssf.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtihvpslcd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtjhmxgksr.html

[E21] 超长截断加省略号
来源：http://hz.xuetiantiany.cn/gthxyvycrv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtlyeqwlqh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tianlin.xyz/gtdvjsigge.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtezgvxqic.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtdtfubutz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtnjzgigfo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guowangkeji.top/gtdhqsorxw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtkfjztlcx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.haohaochexian.top/gtprhlhhyx.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gtlaagheuy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.quarkkingdee.top/gthspdntjk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtifbtdkoz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtdxmrciip.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtfbqldndl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.mhx1999.top/gtvlktzcve.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtgaylxvzq.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigfzy.top/gtihaacqlt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.9152youxi.cn/gtpdzzyjkf.html

================================================================================
来源：http://hz.c1oappe.top/gtraukrvwv.html

F. 文件与目录
来源：http://hz.sxryk.cn/gtblkeqehg.html

================================================================================
来源：http://hz.sweek.top/gtmgakbsvq.html

[F01] 读取整个文件
来源：http://hz.nwbrower.top/gtyniwfqgi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gzhubu.top/gtwboehygn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuetiantiany.cn/gtixxedwjy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangkeji.top/gtwkorxrtl.html


<!-- 参考信息 -->