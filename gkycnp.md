代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.cdnleiting.top/gtkyrzklmx.html

[D16] 求和与平均值
来源：http://hz.hnxiangtu.top/gtfnocgazb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gotoacloud.top/gtbxyxioyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yueranfly.top/gtrdqzhunr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtsuprugtj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtgtzkacxy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gthkjekycs.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtsmlmzfgm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtnvlspdtb.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhoulong.xyz/gtiybmvkdt.html

[D17] 最大值与最小值
来源：http://hz.hfpthk.cn/gtywvdtruf.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtjhtzlqks.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtdxnaydth.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.316326.xyz/gtfznqezcs.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtrtzecdiq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhengqikj.top/gtubrjsohc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dianchejie.cn/gtcubxvzvf.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgfzy.top/gtugmbedzs.html

C#:   list.Max();  list.Min()
来源：http://hz.kuanghao11.cn/gtnutwsslj.html

[D18] 扁平化嵌套数组
来源：http://hz.cheryme.top/gtojvwoked.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gogol.net.cn/gttxyputep.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtvvrrwwmx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yongpay.top/gtfnfzlejv.html

TS:   nested.flat();
来源：http://hz.xingfuxueyuan.xyz/gtpqpstylr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cheryme.top/gttihtwzqz.html

Go:   // 手写双层循环
来源：http://hz.hnqzz.top/gtrqllljwz.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtfrpdsedt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtskvjavbx.html

[D19] 按字段分组
来源：http://hz.gzhubu.top/gtntudelrf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gthggwjqts.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yuxming.cn/gtentbryjy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gtpbvnpcgb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gtoiqrjytw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gtcyrpejez.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gtlioajbcv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtfeklliwo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ehwqpu.com/gtghazfzwc.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtsvccviir.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtrherhqxy.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gteaezkrxl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtfgmenakw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtkyumybie.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hnxiangtu.top/gtsmbidfyu.html

Go:   // 手写 map[T]int
来源：http://hz.xuetiantiany.cn/gtowgcnqck.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtulncudmf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtgiqsufct.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtjoykyjck.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtioobxnum.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtfnpyfvcw.html

JS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtdgwcclkc.html

TS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtpujwjjfh.html

Java: list.contains(x)
来源：http://hz.cheryme.top/gtsppilnjk.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtzapnlbyf.html

Ruby: arr.include?(x)
来源：http://hz.jianghu66.top/gtvpqkpqkr.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtcnreveqo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yangfankeji.com/gtcnlfirvd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.quarkkingdee.top/gtdtmqfzqs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtubsaddhw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yonumen.top/gtbxbmsbnj.html

TS:   [...arr];
来源：http://hz.xingfuxueyuan.xyz/gtvnghtdfq.html

Java: new ArrayList<>(list);
来源：http://hz.hysaishi.cn/gtveunyoxp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenlongwang.top/gtddbqyrji.html

Ruby: arr.dup;  arr.clone
来源：http://hz.kuanghao11.cn/gtlhqdhkqf.html

C#:   new List<int>(list);
来源：http://hz.wangshuangyany.cn/gtxlrmpwyk.html

[D23] reduce 累积计算
来源：http://hz.jqgufenzy.top/gtxbyuuegd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtghtxyplq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yanxiufei.cn/gtviitnhan.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtgjqagkbq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtbsjyjmwn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cheryme.top/gthbgwbnrc.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtqmgfcvnz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtpqtwafdw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gtjmhlexvm.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnqzz.top/gtjnznpaak.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gthgtrbato.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtqbwojghc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.9152youxi.cn/gtqsebmszs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gttybzgtnz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtgcdckdmi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gogol.net.cn/gtwxpnpdes.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daxiang520.top/gtnjhbcajr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenjidiqi.icu/gtuxuhnggq.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gtftkzuxut.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtoiwutcuv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtjznqcytr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jyoumei.cn/gtkpxkinbs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtlddbzixa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ybcxt.top/gtigmyskri.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.c1oappe.top/gtoyrvbzmq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtjuiqyhwc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgfzy.top/gtlgnyujgo.html

[D26] 数组转字符串
来源：http://hz.gogol.net.cn/gtcolarvka.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fzhhl.top/gtrpusqghs.html

PHP:  implode(", ", $arr);
来源：http://hz.xuanzx.com/gtoahqzowj.html

JS:   arr.join(", ")
来源：http://hz.havefunace.top/gtpzqchlav.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtgjedzhnc.html

Java: String.join(", ", list)
来源：http://hz.c1oappe.top/gtabycvgca.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuanzhike.top/gtaftayrrw.html

Ruby: arr.join(", ")
来源：http://hz.jianghu66.top/gtgutlbrkh.html

C#:   string.Join(", ", list)
来源：http://hz.jlsjyb.cn/gtypfyoapp.html

================================================================================
来源：http://hz.xuanzx.com/gtlexdaaxf.html

E. 字符串处理
来源：http://hz.iojbl.cn/gtpxkdoezf.html

================================================================================
来源：http://hz.sweek.top/gtzrfgvcuw.html

[E01] 拼接字符串
来源：http://hz.vqdsnc.cn/gthrubpkfs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cdnleiting.top/gtbhkjauzg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.kuanghao11.cn/gtklsgucxz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gtgkajyqxt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtfmaqocyr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhixingplan.top/gtwklohnsl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cqqwz.cn/gthcwbonbf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gthtpcwaet.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.mhx1999.top/gtlfbuikrl.html

[E02] 重复字符串
来源：http://hz.hfpthk.cn/gtvumskosd.html

Py:   "ab" * 3
来源：http://hz.redwolf501.top/gtrvamwgpr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.snrcjt.cn/gtjrhmfilk.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtdsinpmqa.html

TS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtkjjqemud.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gthvjqqktm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gotoacloud.top/gtdfkjfcfu.html

Ruby: "ab" * 3
来源：http://hz.yanxiufei.cn/gtyrvoidpf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtqneuooim.html

[E03] 截取子串
来源：http://hz.xuanzx.com/gtsiajwile.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cheryme.top/gtictldjrr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.andypj.xyz/gtxaimjcnx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtlogsnozn.html

TS:   s.slice(1, 4)
来源：http://hz.9152youxi.cn/gtdubddnav.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtyxvreooi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aizwys.cn/gtajpwuahw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtryiqjnhn.html

C#:   s.Substring(1, 3)
来源：http://hz.jiagoushi.top/gtiqdrqluv.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtjyvwivcn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtrxvvhjgf.html

PHP:  strpos($s, "x");
来源：http://hz.gzhubu.top/gtscqjfpks.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xziqi.cn/gtfymdrbad.html

TS:   s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtihxaghis.html

Java: s.indexOf("x")
来源：http://hz.cheryme.top/gtkcdzhazh.html

Go:   strings.Index(s, "x")
来源：http://hz.hywenlv.cn/gtwlfyssli.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtgguhhjsa.html

C#:   s.IndexOf("x")
来源：http://hz.yvedp.cn/gtnkakyhlc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhengqikj.top/gtiqkamsbo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.feifeiyinyue.top/gtymcohvbo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tian-w.cn/gtqrpbeesz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtbmxxgltz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hammf.cn/gtbslropaf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtscuemutu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sufxvd.cn/gtscurcatk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xuanzx.com/gtrzsfsjbh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangshuangyany.cn/gtumwomtit.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtnkmguprk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigufen.top/gtutdvagvw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gttddwdjob.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtibjxdjnc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtxnvhpbtq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtjyysbhlw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtdqzoipgt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gaohongyu789.top/gtluhafrvu.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxinkj.top/gthaphovpv.html

[E07] 按分隔符拆分
来源：http://hz.birdmap.top/gtwvczixho.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.0kj1m.cn/gthlrxyeta.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fengsongda.top/gtupggbalp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gtfjovwpdy.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtmtnekyoz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xingfuxueyuan.xyz/gtlpbzbznx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gttrhcxvfz.html

Ruby: s.split(",");  s.split
来源：http://hz.hnqzz.top/gtrrktqehg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.316326.xyz/gtssaskruv.html

[E08] 数组按分隔符合并
来源：http://hz.hammf.cn/gtygobdueo.html

Py:   ",".join(items)
来源：http://hz.jinqigufen.top/gtynxucrvp.html

PHP:  implode(",", $items);
来源：http://hz.yueranfly.top/gtybtmxutu.html

JS:   items.join(",")
来源：http://hz.cheryme.top/gtnjrbexfu.html

TS:   items.join(",")
来源：http://hz.nanxinkj.top/gtxvfjzlhy.html

Java: String.join(",", items)
来源：http://hz.yongpay.top/gtovcfvrcq.html

Go:   strings.Join(items, ",")
来源：http://hz.yueranfly.top/gtqwurcful.html

Ruby: items.join(",")
来源：http://hz.cucudq.cn/gtbrfimcmy.html

C#:   string.Join(",", items)
来源：http://hz.yj202588.top/gtklrkphdm.html

[E09] 去除所有空白字符
来源：http://hz.yanxiufei.cn/gtugwavgwz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gaohongyu789.top/gtdamkuuhd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ybcxt.top/gtmyoktltl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtbbhuyzmr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtsmfglnci.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shzxlz.cn/gtttzarqwr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.52xcode.cn/gtpogtjopk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aizwys.cn/gtfltacfxc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yonumen.top/gtcbksguba.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sufxvd.cn/gthiusobuc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.mhx1999.top/gtczkdaoxw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtfixbnjnn.html

JS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtiabdmjdy.html

TS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtnpvetsxk.html

Java: String.format("%03d", 7)
来源：http://hz.bjfxy.top/gtphgynyrz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtskgtdjyi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hysaishi.cn/gtshchzwer.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yangfankeji.com/gtvvsrvcgf.html

[E11] 反转字符串
来源：http://hz.iojbl.cn/gtzwqrmrnr.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtskduunbn.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gtoblakpnx.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtojitwctn.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtyfxiazsy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtnllscwzz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtokoagmqb.html

Ruby: s.reverse
来源：http://hz.shangyingyoupin.top/gtpcmhxtcu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtvpnvtayl.html

[E12] 统计某字符出现次数
来源：http://hz.jinqigfzy.top/gtedokmgsb.html

Py:   s.count("a")
来源：http://hz.sxryk.cn/gtgngjhzci.html

PHP:  substr_count($s, "a");
来源：http://hz.andypj.xyz/gthhztjekn.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtaxvkahqa.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtamjdbpfv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yvedp.cn/gtydvnwgox.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gthyldtnmv.html

Ruby: s.count("a")
来源：http://hz.jianghu66.top/gttzojjvir.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinghuilouyu.cn/gtaotvrvqe.html

[E13] 逐字符遍历
来源：http://hz.andypj.xyz/gttcrvvaoa.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gtxnsrtlxs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhongyouzk.top/gtsifywisy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtfuaeqwfe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gttwveyrdo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yonumen.top/gtxzxpwmah.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtdhwkkjwh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangshuangyany.cn/gtcuyxomok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtuubornet.html

[E14] URL 编码与 Base64
来源：http://hz.hywenlv.cn/gtocrxdmft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jyoumei.cn/gtdektypip.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtofoljwbn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gtayqrmace.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tian-w.cn/gtolidjujy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ybcxt.top/gttsnoinup.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nwbrower.top/gtzwfdoggt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shangyingyoupin.top/gtfjkveowy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtotfpfiak.html

[E15] HTML 转义 / 反转义
来源：http://hz.yvedp.cn/gthgpugpra.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtzbcwqdoq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daxiang520.top/gthtufozxz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sweek.top/gtofbzhyrz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cucudq.cn/gtgftlhrmu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.quarkkingdee.top/gtresqlsrr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtkcvfknhv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gtntrjjack.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cheryme.top/gtrcvbekcy.html

[E16] 数字千分位
来源：http://hz.chenjidiqi.icu/gtzzpgfchk.html

Py:   f"{1234567:,}"
来源：http://hz.pengpengdd.cyou/gtwrrnmfcg.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtioobusnp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtjibanvmg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtwxdzefgh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yongpay.top/gtdqxbixvb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtnimsowyb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtwjqxgbgz.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gtgqnsszyf.html

[E17] 首字母大写
来源：http://hz.gogol.net.cn/gtdhfbrzni.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtgrsbtfko.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xziqi.cn/gtapnawvby.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gthsqomunx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtxumcjxmj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangshuangyany.cn/gtujiproho.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.havefunace.top/gtvifbjoiw.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtludnxczf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtnszjzxbl.html

[E18] 模板占位符替换
来源：http://hz.guowangkeji.top/gttckttaob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nanxuanxn.top/gtfcbtblkf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtxauotqct.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtcwkxybje.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtbqwvhxap.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zdqjudy.top/gtzqslulop.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangtech.top/gtfcsidqtj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dianchejie.cn/gtjbtoqhrv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtsyehapmv.html

[E19] 多行文本按行拆分
来源：http://hz.fengsongda.top/gtcrjknjii.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gtxvnshfvh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtaimziydt.html

JS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtdvntskgo.html

TS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtxflgpvmg.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtvwcyxxuv.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtosspudpe.html

Ruby: s.lines
来源：http://hz.nanxinkj.top/gtaincskxx.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtojrlxiqp.html

[E20] 判断字符串是否为空
来源：http://hz.zhongyouzk.top/gtcbqcpuvz.html

Py:   if not s:
来源：http://hz.cheryme.top/gtmvulrurs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtfogdonla.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydzc1.top/gtcbeqonfu.html

TS:   if (s === "") {}
来源：http://hz.quarkkingdee.top/gtjnzmbtzi.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtakubsaga.html

Go:   if s == "" {}
来源：http://hz.cucudq.cn/gtgtfgjgxu.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtkhfvkzvd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtgafoavgp.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtzeexklpn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.52xcode.cn/gtcdnicwcv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigfzy.top/gtacphwxzj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gttdxdedtq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtuhlgsyzb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtswrppcng.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shanyushiyangtech.top/gtoxxaxqfh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tanke756.top/gtohfuuaqi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtdkcvvhck.html

[E22] 字节长度与字符长度
来源：http://hz.yangfankeji.com/gtnowbiuhs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtvdmftvhj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtnceqoxjc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gttazlfxxs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtwhjcufqc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gtaswmnexi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuetiantiany.cn/gtcglxetuc.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgufenzy.top/gtavpzkaat.html


<!-- 参考信息 -->