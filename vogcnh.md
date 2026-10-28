代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtwuyhrgnt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj202588.top/gtdgjhzejz.html

TS:   Math.max(...arr);
来源：http://hz.pycfn.com/gtzqbullkn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtccttkibu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aibaodan.cn/gtlhiyzbvs.html

Ruby: arr.max;  arr.min
来源：http://hz.cucudq.cn/gtqcpnscxh.html

C#:   list.Max();  list.Min()
来源：http://hz.vqdsnc.cn/gtbvsglghm.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgufenzy.top/gttsfbiess.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenzaomai.com/gtsdxzlndc.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtkafaxffx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gotoacloud.top/gttzkswmof.html

TS:   nested.flat();
来源：http://hz.xziqi.cn/gtpvskagmq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.smart0.xyz/gtbhdlszqb.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gtrwmruinx.html

Ruby: nested.flatten
来源：http://hz.nanxinkj.top/gtuoxpaxgb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.bjfxy.top/gtvftugdnf.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtadvfywoc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jyoumei.cn/gtdklxpvyc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shzxlz.cn/gtsfqjxlml.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hfpthk.cn/gtlmujnegk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtoevqhnsl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xingfuxueyuan.xyz/gtojsqhdhd.html

Go:   // 手写 map[string][]T
来源：http://hz.daxiang520.top/gtscdxsynu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtaxmztckw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gthoysgwno.html

[D20] 统计每个元素出现次数
来源：http://hz.ydjk.org.cn/gtbhbghbjg.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gtdlvcoakc.html

PHP:  array_count_values($arr);
来源：http://hz.svipenyu.cn/gtwytbvorb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.andypj.xyz/gtrrwdxxtd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtdfljknzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtykxlocds.html

Go:   // 手写 map[T]int
来源：http://hz.daxiang520.top/gtfsttntpq.html

Ruby: arr.tally
来源：http://hz.mhx1999.top/gtvrdqblij.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhengqikj.top/gtsxubophv.html

[D21] 判断是否包含某元素
来源：http://hz.chenzaomai.com/gtcpfbbpwz.html

Py:   x in arr
来源：http://hz.zhiwuduotai.top/gtrgqcggnu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtghpwukci.html

JS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtvrpeoqvd.html

TS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtszkxfnqx.html

Java: list.contains(x)
来源：http://hz.birdmap.top/gtyjcygobi.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtpbnqbojo.html

Ruby: arr.include?(x)
来源：http://hz.cdnleiting.top/gthmalkxuj.html

C#:   list.Contains(x)
来源：http://hz.sufxvd.cn/gtgrnmousf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnqzz.top/gtryzatdip.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhixingplan.top/gtymlulpus.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinghuilouyu.cn/gtqqdeipbi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtxixiztlp.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtigzfljcw.html

Java: new ArrayList<>(list);
来源：http://hz.hongshengwenyu.top/gtcjrhpufi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hfpthk.cn/gtayxnhtkx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtyopkrfps.html

C#:   new List<int>(list);
来源：http://hz.birdmap.top/gtyofnmhli.html

[D23] reduce 累积计算
来源：http://hz.pengpengdd.cyou/gtlpvxrpdn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yangfankeji.com/gtvncghuqw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuanzx.com/gttmpuumhc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gthagmqott.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtzdzepoen.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shuidangran.top/gtikrpmjxj.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtgesnpbsn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gtlqcnhkep.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.dianchejie.cn/gtofykgbtr.html

[D24] 字典 / Map 基本操作
来源：http://hz.cheryme.top/gtgsmnzzsi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtcrqsjfua.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shuidangran.top/gtsmvkspsr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gttnjaqnwp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtugflahsh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guowangkeji.top/gthgsrbxww.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj202588.top/gtsqvnbonw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xingfuxueyuan.xyz/gtbzkrcpfp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gtvnukrirk.html

[D25] Set 集合去重与交并差
来源：http://hz.aizwys.cn/gtfkyonkyc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gtitteobqy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sysykeji.top/gtcyjxgrnt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yanxiufei.cn/gtpekmrnlm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtzxgilsmf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtzifdjadb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pengpengdd.cyou/gtjruffatp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.c1oappe.top/gtobadjltd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hysaishi.cn/gtckyztufv.html

[D26] 数组转字符串
来源：http://hz.yj20258.top/gtysjwpvjf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydzc1.top/gtzknxoqnf.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gtsrtdbzhm.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gttuplaimw.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtqtjxmppw.html

Java: String.join(", ", list)
来源：http://hz.hammf.cn/gthgxskshn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj202588.top/gtsmycdmrl.html

Ruby: arr.join(", ")
来源：http://hz.nanxinkj.top/gtsfppltex.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gttdjqbrvj.html

================================================================================
来源：http://hz.tianlin.xyz/gtjrwobfol.html

E. 字符串处理
来源：http://hz.daria6918.cn/gtmfttmwcd.html

================================================================================
来源：http://hz.hysaishi.cn/gtqkfxbbxn.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtxbmepunv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenjidiqi.icu/gtgdkvndcq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hysaishi.cn/gtobyiunap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtiulmppmm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daxiang520.top/gtucraxmox.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtmbcphtoc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtnwaadtmb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yangfankeji.com/gtrvsgvpqk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhixingplan.top/gthetnekad.html

[E02] 重复字符串
来源：http://hz.hongshengwenyu.top/gtdudgwnjy.html

Py:   "ab" * 3
来源：http://hz.tian-w.cn/gtnfchzqwa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tanke756.top/gtdghsulwa.html

JS:   "ab".repeat(3)
来源：http://hz.hfpthk.cn/gttjjczecd.html

TS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtcojvjhzd.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtshnepznc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cqqwz.cn/gtxqeqzpli.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtoewxjnui.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gotoacloud.top/gtsuhvqsyo.html

[E03] 截取子串
来源：http://hz.zdqjudy.top/gtdywigkwm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtkurhccnt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nwbrower.top/gtbzffsfex.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtaugeupjp.html

TS:   s.slice(1, 4)
来源：http://hz.chenzaomai.com/gtobqwzfqm.html

Java: s.substring(1, 4)
来源：http://hz.ivvv.top/gtugbvxwls.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xinyue.icu/gtlywhbitn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dashuyun.cn/gtqqwixysv.html

C#:   s.Substring(1, 3)
来源：http://hz.zhengqikj.top/gtwjpnrljc.html

[E04] 查找子串位置
来源：http://hz.iojbl.cn/gthfkvgrxa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtgkhyvkzn.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtmucaqigm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yueranfly.top/gtaffssfsb.html

TS:   s.indexOf("x")
来源：http://hz.yuxming.cn/gtheysptmt.html

Java: s.indexOf("x")
来源：http://hz.zycfv.cn/gtglxxzmzm.html

Go:   strings.Index(s, "x")
来源：http://hz.ybcxt.top/gtflloxrnm.html

Ruby: s.index("x")
来源：http://hz.sxryk.cn/gtkzflrfuw.html

C#:   s.IndexOf("x")
来源：http://hz.zhiwuduotai.top/gtxlboxkuc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hfpthk.cn/gtrxafqibj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtngejahyc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinghuilouyu.cn/gthrukdazo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guowangkeji.top/gtpqdplvur.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ybcxt.top/gtpwhnypkt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtasltmexb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtbzfxmyjv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ywan-chungtsiang.top/gtknclnveh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.316326.xyz/gtaxwewhki.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtsfbhvqfh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hfpthk.cn/gtigoisaae.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yvedp.cn/gtdmryqcxa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gthsjjetbv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtoopdkpal.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtcbdjcpbq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.redwolf501.top/gthlybryqs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.mhx1999.top/gtuliikykb.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gtyhlazdal.html

[E07] 按分隔符拆分
来源：http://hz.yvedp.cn/gtflwjitjl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cashguo.top/gtkpkpzxzb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xylfe.cn/gteocoimch.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sufxvd.cn/gtvwgwvark.html

TS:   s.split(",")
来源：http://hz.shanyushiyangkeji.top/gtqgevuoop.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.9152youxi.cn/gthumjcgbr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gthzijaarq.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtprumbtqx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tanke756.top/gtvztqgste.html

[E08] 数组按分隔符合并
来源：http://hz.xuanzx.com/gtrdqarjlp.html

Py:   ",".join(items)
来源：http://hz.jqgfzy.top/gtvxpfjrdh.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtbxmivbkg.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gthgspexpk.html

TS:   items.join(",")
来源：http://hz.yvedp.cn/gtivmnkrot.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gttlbvvdgo.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtgdbuamkz.html

Ruby: items.join(",")
来源：http://hz.zycfv.cn/gtsedaodjl.html

C#:   string.Join(",", items)
来源：http://hz.ybcxt.top/gtnxhdrzbz.html

[E09] 去除所有空白字符
来源：http://hz.jlsjyb.cn/gtflypxecd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtzxjlmiyn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.redwolf501.top/gtwkkgltye.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtobphhycu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sufxvd.cn/gtvvtnrdwy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zycfv.cn/gtktwyffbt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jyoumei.cn/gteuxsjeum.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtljrvxhtt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xylfe.cn/gtbuvmclib.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yanxiufei.cn/gtcfflzgri.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuetiantiany.cn/gtetvglmlh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tian-w.cn/gtbibujmpk.html

JS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtubsppsgf.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtuvvcjrhr.html

Java: String.format("%03d", 7)
来源：http://hz.pycfn.com/gtyjpuixzn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtswddjsdq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtuanmsidw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yongpay.top/gtvakdwtqw.html

[E11] 反转字符串
来源：http://hz.daxiang520.top/gtprxfpcrq.html

Py:   s[::-1]
来源：http://hz.ybcxt.top/gtrnicsnts.html

PHP:  strrev($s);
来源：http://hz.shzxlz.cn/gtndflzxnh.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtsrdmeqvj.html

TS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtsrytsozt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jiagoushi.top/gtntlgnxha.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangtech.top/gtcazamzmw.html

Ruby: s.reverse
来源：http://hz.yuanzhike.top/gtgetvursx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtgnhdwcfj.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258.top/gtnyfbhjjp.html

Py:   s.count("a")
来源：http://hz.xuetiantiany.cn/gtkvicrpzm.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtbzwszhuj.html

JS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gteoaqvvpu.html

TS:   s.split("a").length - 1
来源：http://hz.xuetiantiany.cn/gtseonjzuk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shanyushiyangkeji.top/gtyqskeujr.html

Go:   strings.Count(s, "a")
来源：http://hz.xziqi.cn/gtkqhcscwo.html

Ruby: s.count("a")
来源：http://hz.cqqwz.cn/gtbzpgwseg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj202588.top/gthzwydprd.html

[E13] 逐字符遍历
来源：http://hz.cucudq.cn/gtvizlpcfp.html

Py:   for ch in s: print(ch)
来源：http://hz.ywan-chungtsiang.top/gtitkyzxni.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtewuwyjvy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtimohyehv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gttoengylb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gthhbagesm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.c1oappe.top/gtqflyfktl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenlongwang.top/gtkrcudpiu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258.top/gthwxmdhkg.html

[E14] URL 编码与 Base64
来源：http://hz.guannengcc.top/gtsdsrecfk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxuanxn.top/gtfhzlvheg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daria6918.cn/gtrkqiejbb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gtiuxomrvy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangtech.top/gtrxhquuwk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtvolsybtx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigfzy.top/gtcmfjfyvr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xziqi.cn/gtunuhxohr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cashguo.top/gttxedyvez.html

[E15] HTML 转义 / 反转义
来源：http://hz.aizwys.cn/gtiiczjxkl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangkeji.top/gtwxjdkdro.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sweek.top/gtonmbdwai.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuxming.cn/gtggwlumma.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenzaomai.com/gtvkpxaveg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj202588.top/gtxzrnxnur.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gtldaqlzwq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gzhubu.top/gthzrdqrwa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gthcqsgkuo.html

[E16] 数字千分位
来源：http://hz.ydjk.org.cn/gtgtzpvmig.html

Py:   f"{1234567:,}"
来源：http://hz.gzhubu.top/gtuypejbnn.html

PHP:  number_format(1234567);
来源：http://hz.cucudq.cn/gtppwtpbjp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtyovzyoaw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtuwjlkyws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cucudq.cn/gtzehvgzaq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtpptwnstg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhaomingkeji.xyz/gtpxhffmhw.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gteappafbx.html

[E17] 首字母大写
来源：http://hz.havefunace.top/gtyrcyyovl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhengqikj.top/gtztwbvabl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtlqmznwxc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtxysthapo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gtknxuolzl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ywan-chungtsiang.top/gtwvokqibw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinyuanbaomall.cn/gtyptvvpyz.html

Ruby: s.capitalize
来源：http://hz.yangfankeji.com/gtvlgxuxgo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zycfv.cn/gtrkilzgsx.html

[E18] 模板占位符替换
来源：http://hz.zycfv.cn/gtoinoagvi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fzhhl.top/gtuggarncv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtuxgjatad.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtexylcfhg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtqhexsrbo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhijiandao.cn/gtarfwnufb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gthdmjfbxq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pengpengdd.cyou/gtljjnqfnd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtthxcxlqh.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtslcbgmin.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtfwnenfav.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aibaodan.cn/gtrllcvpvl.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtnvvsipif.html

TS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gthwqscmwe.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtwuodphpo.html

Go:   strings.Split(s, "\n")
来源：http://hz.birdmap.top/gtvjckmrvp.html

Ruby: s.lines
来源：http://hz.sysykeji.top/gtcvdetajv.html

C#:   s.Split('\n')
来源：http://hz.c1oappe.top/gtpulrwilb.html

[E20] 判断字符串是否为空
来源：http://hz.gzhubu.top/gtqkuqndbz.html

Py:   if not s:
来源：http://hz.jinyuanbaomall.cn/gtefpnqqjs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtbwplgapd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.smart0.xyz/gtyxvafvdf.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtveqylybb.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangdashe.top/gthvofcjcz.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gtilnospkx.html

Ruby: if s.empty?
来源：http://hz.meibo888.top/gtqjsvozue.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gtaujxdiib.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtqcbcljzt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yueranfly.top/gthejuokkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shuidangran.top/gtkdxhjwni.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtknglryky.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gteacdljrg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtnmzdrvns.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cashguo.top/gtiseuxyxd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gaohongyu789.top/gtproiuhdf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gtdhlgggdc.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gtyhihvdjn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ehwqpu.com/gtghkguhlh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jiagoushi.top/gtwvodxygs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtsokoywxi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtyzifodrg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtetaevhwo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dashuyun.cn/gtiiwawdbg.html

Ruby: s.bytesize;  s.length
来源：http://hz.vqdsnc.cn/gtxdkkxjhi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gttyngcmfi.html

================================================================================
来源：http://hz.chenlongwang.top/gtupycxxvg.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gthjvrviig.html

================================================================================
来源：http://hz.nanxuanxn.top/gtlgliaewl.html

[F01] 读取整个文件
来源：http://hz.nanxuanxn.top/gtyxcbqosv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.9152youxi.cn/gtthenlnki.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtrfofmxvr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zdqjudy.top/gteybwrjin.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.andypj.xyz/gtkxptrtrw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gthsgkjwve.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cheryme.top/gtcciajmgo.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtfzrxwdwm.html


<!-- 参考信息 -->