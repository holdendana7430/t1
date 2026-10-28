代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.cheryme.top/gtdiitbcmy.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gtauzbzpia.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhongyouzk.top/gtmgibddih.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ybcxt.top/gtlwqgzblk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtaktczcox.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtqlmmplwk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gotoacloud.top/gtpurlgngv.html

Go:   // 手写循环累加
来源：http://hz.hongshengwenyu.top/gtzzcnizvz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gaohongyu789.top/gtztjtoxub.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtpaapuchh.html

[D17] 最大值与最小值
来源：http://hz.smart0.xyz/gtltidzbwd.html

Py:   max(arr);  min(arr)
来源：http://hz.redwolf501.top/gtfriqlosz.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtrpbotzhs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pycfn.com/gteezunhsc.html

TS:   Math.max(...arr);
来源：http://hz.zhoulong.xyz/gtqnqlitvz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cdnleiting.top/gtuzmezatt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.snrcjt.cn/gtdnitjbtn.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtdztcxkpc.html

C#:   list.Max();  list.Min()
来源：http://hz.snrcjt.cn/gtcglrhgye.html

[D18] 扁平化嵌套数组
来源：http://hz.daxiang520.top/gtdnmqafab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guannengcc.top/gtpsvhhfnl.html

PHP:  array_merge(...$nested);
来源：http://hz.sysykeji.top/gtitpipois.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtloasqjwp.html

TS:   nested.flat();
来源：http://hz.birdmap.top/gtciayltcy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.bjfxy.top/gtqjliezoe.html

Go:   // 手写双层循环
来源：http://hz.ppjwa.cn/gtnrnjtzhy.html

Ruby: nested.flatten
来源：http://hz.tanke756.top/gtymqngfik.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj202588.top/gtmdpbwpvq.html

[D19] 按字段分组
来源：http://hz.quarkkingdee.top/gtllfdftin.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.meibo888.top/gtpdrzszmu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinqigfzy.top/gtjslpefii.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xinyue.icu/gtlziyubop.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtqmmkthli.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gtchajyypi.html

Go:   // 手写 map[string][]T
来源：http://hz.mhx1999.top/gtsuykyush.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydzc1.top/gtkzwfnigb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tanke756.top/gtcsexugdv.html

[D20] 统计每个元素出现次数
来源：http://hz.hfpthk.cn/gtennmowvw.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gtbyazopji.html

PHP:  array_count_values($arr);
来源：http://hz.ydjk.org.cn/gtealyzuil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtufmqolay.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gttnfsjaee.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cheryme.top/gtnxcrptug.html

Go:   // 手写 map[T]int
来源：http://hz.snrcjt.cn/gtkjhbsxfu.html

Ruby: arr.tally
来源：http://hz.yuanzhike.top/gtwaorsebn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aizwys.cn/gtkqakxjva.html

[D21] 判断是否包含某元素
来源：http://hz.xinyue.icu/gtkdynzxyl.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtqvwayvjm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gtduutzmfd.html

JS:   arr.includes(x)
来源：http://hz.wangdashe.top/gtqnqkwbvc.html

TS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtevmxulag.html

Java: list.contains(x)
来源：http://hz.ybcxt.top/gtwyangxij.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuanzx.com/gtsqywlopy.html

Ruby: arr.include?(x)
来源：http://hz.ehwqpu.com/gtlniixajw.html

C#:   list.Contains(x)
来源：http://hz.xinyue.icu/gtrlgfvhet.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jlsjyb.cn/gtjtznrgbv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.birdmap.top/gtetwbmzhw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuxming.cn/gtpgkkpjce.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jianghu66.top/gtaegndljf.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtjswcznxe.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtihuewyhi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhixingplan.top/gtmimhjhoq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxuanxn.top/gtidnflssc.html

C#:   new List<int>(list);
来源：http://hz.tianlin.xyz/gtzkapfoys.html

[D23] reduce 累积计算
来源：http://hz.gaohongyu789.top/gtsrfmgkzp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhaomingkeji.xyz/gtokjggyoi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nwbrower.top/gtqauukogn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtjxjaeahu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtqtfpjson.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gtxjqdwboc.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gtvjsdgglk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hongshengwenyu.top/gtuzcwkxwh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yonumen.top/gtmgyhzbbr.html

[D24] 字典 / Map 基本操作
来源：http://hz.cqqwz.cn/gtepcuuztu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cucudq.cn/gtafgtbkse.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinghuilouyu.cn/gthrjcbndr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtaxwygmxz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtxsglemrd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtixlmguio.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgufenzy.top/gtlnvdvvuc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gttfzyyfmn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xinyue.icu/gtpltrughf.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258888.top/gtiyindkki.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cqqwz.cn/gtuwyicvxe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtojxnvowq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtxygtbqkx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhijiandao.cn/gtwpgtpfhf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtgrpgnozs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tianlin.xyz/gtgrcssqwq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.birdmap.top/gtjsktalun.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.0kj1m.cn/gtogbenjbr.html

[D26] 数组转字符串
来源：http://hz.316326.xyz/gtfcosbbxz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtcucugliu.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gtmqdmbkax.html

JS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtjuuftwqu.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtsqzxkjru.html

Java: String.join(", ", list)
来源：http://hz.gogol.net.cn/gtrcntxtne.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sysykeji.top/gtzceckhzo.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gthcymxhin.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtvwoygpxb.html

================================================================================
来源：http://hz.yj20258.top/gtfmrqyqgk.html

E. 字符串处理
来源：http://hz.zhengqikj.top/gtghtpgtnt.html

================================================================================
来源：http://hz.tian-w.cn/gthlmzcczf.html

[E01] 拼接字符串
来源：http://hz.daxiang520.top/gtpcqhgtgg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtpsmjfcfw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtpejarsmy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fzhhl.top/gteaicoaqg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtmkcduqod.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtbxcstlxv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangtech.top/gtwgkyucho.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydzc1.top/gtrvjydosi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtpvyfmqsh.html

[E02] 重复字符串
来源：http://hz.jlsjyb.cn/gtbszurabz.html

Py:   "ab" * 3
来源：http://hz.shanyushiyangtech.top/gteozlvnke.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtlzvjxcvi.html

JS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtyvhhthka.html

TS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtrieugsvp.html

Java: "ab".repeat(3)
来源：http://hz.cashguo.top/gtregpoqbj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ydzc1.top/gtwwbfnzku.html

Ruby: "ab" * 3
来源：http://hz.svipenyu.cn/gtusgmkjpw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtozivqkyg.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtfwtpchbu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtepbkmubt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigufen.top/gttrxufktv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtyoqjnwbe.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gthoaetocq.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtwpttxnij.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuxming.cn/gtylcoadau.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuanzhike.top/gtnkpfcliv.html

C#:   s.Substring(1, 3)
来源：http://hz.shzxlz.cn/gtaitnatts.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gtxvwisdus.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tianlin.xyz/gtuiflegwe.html

PHP:  strpos($s, "x");
来源：http://hz.birdmap.top/gtsywcajjp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhoulong.xyz/gtqunxpmik.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtvplwewjm.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangtech.top/gtsgmxwkpz.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgfzy.top/gtiuqiszer.html

Ruby: s.index("x")
来源：http://hz.ydjk.org.cn/gtcgvgfdni.html

C#:   s.IndexOf("x")
来源：http://hz.fzhhl.top/gttmtkveuu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xylfe.cn/gtwxwdvbmd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.316326.xyz/gtzwsfpbto.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtoiajscka.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtxhxpwwmb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnqzz.top/gtcbpebjwx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtzhjyvvkj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gaohongyu789.top/gtebwfelvr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zdqjudy.top/gtfardlrzk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shangyingyoupin.top/gtevtumtji.html

[E06] 替换子串
来源：http://hz.xingfuxueyuan.xyz/gtwtgotyvo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhengqikj.top/gtjyryfuhp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xinyue.icu/gtuzswacgd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtfdstlqsc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtplmnphnv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtwwpbvqfi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtewhawiis.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shanyushiyangtech.top/gtfzanvane.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigufen.top/gtoekszdpo.html

[E07] 按分隔符拆分
来源：http://hz.tianlin.xyz/gtjoroosli.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangtech.top/gtcgznupzn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.meibo888.top/gtebaqlzyy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gtpuflhzfj.html

TS:   s.split(",")
来源：http://hz.ydjk.org.cn/gtixxmbsjj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtpsrnwryt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xziqi.cn/gtuhagynwt.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangkeji.top/gtmkkpqwqp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sxryk.cn/gteaqokyrr.html

[E08] 数组按分隔符合并
来源：http://hz.c1oappe.top/gtodfigzzw.html

Py:   ",".join(items)
来源：http://hz.ivvv.top/gtgzpqsvgq.html

PHP:  implode(",", $items);
来源：http://hz.fengsongda.top/gtypiwihcy.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtairjstxc.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtsdlbmfsi.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtdowosalf.html

Go:   strings.Join(items, ",")
来源：http://hz.cheryme.top/gtwglqbodn.html

Ruby: items.join(",")
来源：http://hz.dianchejie.cn/gtfvnilmco.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangtech.top/gtnizpldwd.html

[E09] 去除所有空白字符
来源：http://hz.pycfn.com/gtkdtwygcp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yvedp.cn/gtjmqptqeo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtgruxlhen.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtnosnyxgg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtnwwkphpg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtluioaneu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhoulong.xyz/gtirntfyns.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtycpyajpc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtjagacang.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtrnsbrqjv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sysykeji.top/gtzbgzwbnf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.9152youxi.cn/gtncuyalcw.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtknzbpuyx.html

TS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gthkihuuew.html

Java: String.format("%03d", 7)
来源：http://hz.shzxlz.cn/gtwijkibch.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gtoskqajzg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtidekwjvi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.mhx1999.top/gtbqzzopdk.html

[E11] 反转字符串
来源：http://hz.shanyushiyangtech.top/gtnlgeswrm.html

Py:   s[::-1]
来源：http://hz.jyoumei.cn/gtzxlaigou.html

PHP:  strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtgjslzouv.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtlyobpkoo.html

TS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtrttqised.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tianlin.xyz/gtzjftzyqv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shuidangran.top/gteogonpmg.html

Ruby: s.reverse
来源：http://hz.ybcxt.top/gthgigouwc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtpxcoawiy.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtwbciigqr.html

Py:   s.count("a")
来源：http://hz.dashuyun.cn/gtvcvqfqgu.html

PHP:  substr_count($s, "a");
来源：http://hz.xinyue.icu/gtojtamjbt.html

JS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtdyawxviw.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtbfgrkaaf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtpxmiujoy.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtxxnvogfy.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtjkvfkeev.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zdqjudy.top/gtpyexijri.html

[E13] 逐字符遍历
来源：http://hz.shangyingyoupin.top/gtbxlzimvx.html

Py:   for ch in s: print(ch)
来源：http://hz.bjfxy.top/gturgtwqrk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.snrcjt.cn/gtdytwuxxs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cashguo.top/gttizgqrff.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtpneanman.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtrtupbuxy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ppjwa.cn/gtuoriuuiw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtmsbleiks.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgfzy.top/gtdukqwibi.html

[E14] URL 编码与 Base64
来源：http://hz.nwbrower.top/gthuxctliu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.vqdsnc.cn/gtssmqidvr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sufxvd.cn/gtvxrmbnkv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtdoryvumf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhixingplan.top/gtngtjpmmt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.0kj1m.cn/gtbqfodacl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhixingplan.top/gteahcizdq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtqavilsjh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.bjfxy.top/gtdrnatlwf.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenlongwang.top/gtlicaauae.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pycfn.com/gtowgycuwd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuanzhike.top/gtmzztnooa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtfbscsbbf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtkyzcrpxi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sufxvd.cn/gtsaqjcmcj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aizwys.cn/gtbvctycrn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gthfykzque.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhiwuduotai.top/gtbnxxxuex.html

[E16] 数字千分位
来源：http://hz.tanke756.top/gtigjqcvfj.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtvfymfcog.html

PHP:  number_format(1234567);
来源：http://hz.vqdsnc.cn/gtryhaxfux.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtvbzxuibs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.smart0.xyz/gtcxkswfaf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtrplxzhhs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ywan-chungtsiang.top/gttgglphmp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gtptnaxdbu.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtjwzhvjyg.html

[E17] 首字母大写
来源：http://hz.vqdsnc.cn/gtrqgsfwii.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hongshengwenyu.top/gtcbmxumkj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgfzy.top/gtptznkgkl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtgkcwctjt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtduvqutva.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hongshengwenyu.top/gtrjebqere.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtyfxzfzou.html

Ruby: s.capitalize
来源：http://hz.yongpay.top/gtbucmgnec.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gtdnftqsqn.html

[E18] 模板占位符替换
来源：http://hz.zhoulong.xyz/gtfvaxuffp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258.top/gtahbpcuqa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.havefunace.top/gtysrzbrgg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtndekvgle.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gttalgnnwu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtpftrpezm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fzhhl.top/gtbkbrdjuw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtelefcvet.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigfzy.top/gtkzgnbpui.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtceflpbki.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gtezjtdhbk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj202588.top/gtuqmvyqhb.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhaomingkeji.xyz/gtjdawoolw.html

TS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtetqefdlj.html

Java: s.lines().toList()
来源：http://hz.ehwqpu.com/gtylatrulp.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtkjyuvbon.html

Ruby: s.lines
来源：http://hz.shuidangran.top/gtmndyigew.html

C#:   s.Split('\n')
来源：http://hz.jqgfzy.top/gtveklptek.html

[E20] 判断字符串是否为空
来源：http://hz.zycfv.cn/gtivpeojhu.html

Py:   if not s:
来源：http://hz.yj20258.top/gtovntzmpg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ybcxt.top/gtztpltlxx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258888.top/gtwnlduqew.html

TS:   if (s === "") {}
来源：http://hz.gotoacloud.top/gtudpdgfns.html

Java: if (s.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtnqaxysno.html

Go:   if s == "" {}
来源：http://hz.feifeiyinyue.top/gthelrglvg.html

Ruby: if s.empty?
来源：http://hz.dashuyun.cn/gtsmgiooin.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtgrmjgdmn.html

[E21] 超长截断加省略号
来源：http://hz.zhongyouzk.top/gtrefllzcs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtmtlzlogh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.feifeiyinyue.top/gtnrrlavmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtfgeghige.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gttxnlotxb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtiiiktutk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtejnkonpw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sxryk.cn/gtadltrgry.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guowangkeji.top/gtsfimmgro.html

[E22] 字节长度与字符长度
来源：http://hz.ivvv.top/gtvpnbldas.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tanke756.top/gtszuksmsu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtlcyruifg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtsiwahymx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtwpfdtbxd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nwbrower.top/gtbbrjeizl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtysxitphb.html

Ruby: s.bytesize;  s.length
来源：http://hz.nwbrower.top/gtexhwjrgr.html


<!-- 参考信息 -->