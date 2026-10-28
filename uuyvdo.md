代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtezwsnwzt.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gtjnhhhwib.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigufen.top/gtjfruzust.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtozydaard.html

[D15] 去重
来源：http://hz.guowangkeji.top/gtapqjqmly.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtqnjtqgpv.html

PHP:  array_unique($arr);
来源：http://hz.xylfe.cn/gtzzjjnbiu.html

JS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtvntpgzyx.html

TS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtyjmhpjkj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtalseztyk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.c1oappe.top/gtbyxxzmdw.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtbwhiwltp.html

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gtfsuarywf.html

[D16] 求和与平均值
来源：http://hz.nanxinkj.top/gtaoixskat.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.c1oappe.top/gtnidxpqrh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ivvv.top/gtakskdgav.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtyeqoaziv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jyoumei.cn/gthgmwmyde.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tanke756.top/gtieydqzle.html

Go:   // 手写循环累加
来源：http://hz.hongshengwenyu.top/gtbujigpze.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gtqhkgudgx.html

C#:   list.Sum();  list.Average()
来源：http://hz.sweek.top/gtsqxistvz.html

[D17] 最大值与最小值
来源：http://hz.yueranfly.top/gtyierwkqz.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtijqvolic.html

PHP:  max($arr);  min($arr);
来源：http://hz.gaohongyu789.top/gtbdabfzta.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zdqjudy.top/gtrtovzhzi.html

TS:   Math.max(...arr);
来源：http://hz.aibaodan.cn/gtnbdoainu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aizwys.cn/gtpllbzbcb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cashguo.top/gthjdnyafs.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtivqrivik.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtmkrlhmxl.html

[D18] 扁平化嵌套数组
来源：http://hz.aizwys.cn/gtasqhurrr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtzisjzhvx.html

PHP:  array_merge(...$nested);
来源：http://hz.chenjidiqi.icu/gtibppmzeh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.haohaochexian.top/gtyjlojczd.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtrypmcenx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aibaodan.cn/gtkcypfzwy.html

Go:   // 手写双层循环
来源：http://hz.xingfuxueyuan.xyz/gtiojykajl.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtrhnosbda.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtunmqjnhp.html

[D19] 按字段分组
来源：http://hz.yuxming.cn/gtrarbwsrs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gthkzseomd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenzaomai.com/gtinfvqsga.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.9152youxi.cn/gtpdayeldl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtauiwonzl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.smart0.xyz/gtolxyjdna.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gtkmnnhpjh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.kuanghao11.cn/gtysmpcxjn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtxqqtktnc.html

[D20] 统计每个元素出现次数
来源：http://hz.ydzc1.top/gtcfwxouih.html

Py:   Counter(arr)
来源：http://hz.andypj.xyz/gtjvdieags.html

PHP:  array_count_values($arr);
来源：http://hz.gaohongyu789.top/gthogrsmbi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtgfrlmdpi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtgffoafzv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hywenlv.cn/gtraijmikv.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gtgivdbdvo.html

Ruby: arr.tally
来源：http://hz.9152youxi.cn/gtyisltzjz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydzc1.top/gtxybqutsl.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtghljciwt.html

Py:   x in arr
来源：http://hz.ydzc1.top/gtbpdfusuy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daria6918.cn/gtfromxdht.html

JS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gterznpwmn.html

TS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtstjgkizr.html

Java: list.contains(x)
来源：http://hz.cucudq.cn/gtmrepapua.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtupwhlevr.html

Ruby: arr.include?(x)
来源：http://hz.cqqwz.cn/gtmswcvmbm.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gtxfcgnivo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtmrqexfck.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.havefunace.top/gtonpmvyma.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.bjfxy.top/gtqqupneam.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shangyingyoupin.top/gtexeafugf.html

TS:   [...arr];
来源：http://hz.c1oappe.top/gtvruvqfbc.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtpzgetluu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigufen.top/gttwntzqiq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuxming.cn/gtqcxcufbp.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtiptmliwb.html

[D23] reduce 累积计算
来源：http://hz.sysykeji.top/gttesntgut.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yongpay.top/gtlibnseou.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zycfv.cn/gtnnadpgoa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenzaomai.com/gtxfppylot.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtgbqjhoyl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hywenlv.cn/gtplyiclax.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtjlwnvexj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtkkqevjul.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtgejfymwq.html

[D24] 字典 / Map 基本操作
来源：http://hz.0kj1m.cn/gtwrsdhfjp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydzc1.top/gtrpxkkkdw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xingfuxueyuan.xyz/gtoqsooojd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj202588.top/gtmcvclzfa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj202588.top/gtwytljint.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhaomingkeji.xyz/gtnxhgmqyv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtqtehunoa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtzpkjaenc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gtyzauuhyo.html

[D25] Set 集合去重与交并差
来源：http://hz.jinghuilouyu.cn/gtrhqumdof.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtqgebzaqn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fengsongda.top/gtjocsigoj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxinkj.top/gtkvhltgrd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zdqjudy.top/gtxsvozjis.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.quarkkingdee.top/gtmnpunfal.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jyoumei.cn/gtxnpkjtep.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hongshengwenyu.top/gtnnuoqydp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gttmewquze.html

[D26] 数组转字符串
来源：http://hz.mhx1999.top/gtstcqvomh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangshuangyany.cn/gtotzavjup.html

PHP:  implode(", ", $arr);
来源：http://hz.zhaomingkeji.xyz/gtabipmgeq.html

JS:   arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtmyipijjp.html

TS:   arr.join(", ")
来源：http://hz.vqdsnc.cn/gtpbpvzbfs.html

Java: String.join(", ", list)
来源：http://hz.shuidangran.top/gtwzavosox.html

Go:   strings.Join(strs, ", ")
来源：http://hz.haohaochexian.top/gttxccuvbq.html

Ruby: arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gttjujexvs.html

C#:   string.Join(", ", list)
来源：http://hz.nwbrower.top/gtkpwsubaf.html

================================================================================
来源：http://hz.xuanzx.com/gtgnhdapgk.html

E. 字符串处理
来源：http://hz.daxiang520.top/gtmisjlsfz.html

================================================================================
来源：http://hz.yj20258888.top/gtjuopwlzi.html

[E01] 拼接字符串
来源：http://hz.hongshengwenyu.top/gtmikoxcab.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.vqdsnc.cn/gtxkieznnt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenjidiqi.icu/gtqukdunuy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtmxtbpakw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtmunfdjvp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.kuanghao11.cn/gtezvrqsqf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tianlin.xyz/gtvaaexwaz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tianlin.xyz/gtmbzduhvs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.iojbl.cn/gtagxsmokd.html

[E02] 重复字符串
来源：http://hz.cashguo.top/gtqdcigtot.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtxtfapans.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gtbcsgalvj.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtftfftuvk.html

TS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gtpeizxpkx.html

Java: "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtnieqkyiw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gturwoekiv.html

Ruby: "ab" * 3
来源：http://hz.tanke756.top/gtpbbiagoj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.snrcjt.cn/gtxkfgdnvg.html

[E03] 截取子串
来源：http://hz.c1oappe.top/gtycaowray.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cheryme.top/gtwsaqhowc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigfzy.top/gtwjhcrfhw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gthozevxxi.html

TS:   s.slice(1, 4)
来源：http://hz.zhongyouzk.top/gtvxuauvde.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtjprucxno.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daria6918.cn/gtwwjynoht.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gthievghhq.html

C#:   s.Substring(1, 3)
来源：http://hz.cdnleiting.top/gtxuzcojus.html

[E04] 查找子串位置
来源：http://hz.daria6918.cn/gtxysultcy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xziqi.cn/gtkofyafgz.html

PHP:  strpos($s, "x");
来源：http://hz.gzhubu.top/gtvmbdikbs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hfpthk.cn/gtwldjqvkn.html

TS:   s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtwaltpvkc.html

Java: s.indexOf("x")
来源：http://hz.xuanzx.com/gtyznmuzea.html

Go:   strings.Index(s, "x")
来源：http://hz.cdnleiting.top/gtprzdxkvh.html

Ruby: s.index("x")
来源：http://hz.jinqigufen.top/gthnfwrlwj.html

C#:   s.IndexOf("x")
来源：http://hz.andypj.xyz/gtvrlmnpmy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhijiandao.cn/gtvqotzbtk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhijiandao.cn/gtwazrosqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xingfuxueyuan.xyz/gttdaugril.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtkujdccog.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.52xcode.cn/gtaqanikeq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gotoacloud.top/gtnftitcfk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zycfv.cn/gtfevnlirx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daxiang520.top/gttffojuze.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zycfv.cn/gtwvbixypr.html

[E06] 替换子串
来源：http://hz.yonumen.top/gtlutrlkxl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.aizwys.cn/gtodgyxrgx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xylfe.cn/gtqbffyuen.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtggtygluk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtsydzlxjh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gttyqtqtjt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhixingplan.top/gttzfjprtl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jianghu66.top/gtqggyfvit.html

C#:   s.Replace("a", "b")
来源：http://hz.9152youxi.cn/gtsbplpoqy.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtjsmzttsr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj202588.top/gtkxsxscfr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sxryk.cn/gttdeiueef.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhoulong.xyz/gtffiasdyu.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtfgcirqia.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuetiantiany.cn/gtzuiqkxsn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jqgfzy.top/gtrxtlhgfn.html

Ruby: s.split(",");  s.split
来源：http://hz.ydzc1.top/gtmkfylwbs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.birdmap.top/gtrvvqaehu.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gthsgozmuk.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gtkklsafez.html

PHP:  implode(",", $items);
来源：http://hz.ybcxt.top/gtiktvarur.html

JS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtphhulgjx.html

TS:   items.join(",")
来源：http://hz.sufxvd.cn/gtmanybthc.html

Java: String.join(",", items)
来源：http://hz.mhx1999.top/gtstmknbfe.html

Go:   strings.Join(items, ",")
来源：http://hz.chenzaomai.com/gtzymddihm.html

Ruby: items.join(",")
来源：http://hz.quarkkingdee.top/gtwnaykann.html

C#:   string.Join(",", items)
来源：http://hz.ydjk.org.cn/gtnchhkyyu.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtqxtoaxbr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenjidiqi.icu/gtbqceycrd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sxryk.cn/gtcznjjiqj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtswrtqqya.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtlenqrtls.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhongyouzk.top/gtlmiqoyae.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hnqzz.top/gtfcewpkzf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sweek.top/gtjkscdiri.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ybcxt.top/gtyiczlyda.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtmfxlcuqy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtdecjwler.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.snrcjt.cn/gtpgujctpe.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtrnakeeib.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtrotdcawk.html

Java: String.format("%03d", 7)
来源：http://hz.daxiang520.top/gtiikxxwac.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtqmqkbmbz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258.top/gtkackfdqa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgufenzy.top/gtzqhgydos.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gthkflkpnz.html

Py:   s[::-1]
来源：http://hz.nanxinkj.top/gtyedakhzz.html

PHP:  strrev($s);
来源：http://hz.fengsongda.top/gtwlwnxqup.html

JS:   [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtrirbzhbv.html

TS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtuuztkcky.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yongpay.top/gtlfviwexu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhaomingkeji.xyz/gtgijnledh.html

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtbmepikyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtpqoxnoyw.html

[E12] 统计某字符出现次数
来源：http://hz.fengsongda.top/gtwdrgibjb.html

Py:   s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtzszjssog.html

PHP:  substr_count($s, "a");
来源：http://hz.gaohongyu789.top/gtiisafdpy.html

JS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtarkumgya.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtjwxohpuy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gtvlrydbxy.html

Go:   strings.Count(s, "a")
来源：http://hz.havefunace.top/gtnmhzkbwd.html

Ruby: s.count("a")
来源：http://hz.cqqwz.cn/gtgxzzpsnk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gtaftucrum.html

[E13] 逐字符遍历
来源：http://hz.jinghuilouyu.cn/gtvyhokjha.html

Py:   for ch in s: print(ch)
来源：http://hz.hammf.cn/gtxmxwtbvu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.snrcjt.cn/gtgsufbrku.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtfhoqjkgj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtfmoblity.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gttkdfkguk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhijiandao.cn/gtxpxybcdk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangshuangyany.cn/gtrsmyheok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yueranfly.top/gtvroczfei.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtbevjnnej.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtgnolzptq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gtoqyedumb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gthhkrruhp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangkeji.top/gtatouaima.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tian-w.cn/gtuparzabx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fzhhl.top/gtcusjvive.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtdictzrzv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenzaomai.com/gtcnvnvojl.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangshuangyany.cn/gtpaatkbrb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gtzvrlczqo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guowangkeji.top/gtpvsymcsu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gtopqovtcn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtpjyaacyu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gotoacloud.top/gtlosjmbmn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gturwfpwxy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtolwnzagf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtabzghdkz.html

[E16] 数字千分位
来源：http://hz.fzhhl.top/gtmchuvwnc.html

Py:   f"{1234567:,}"
来源：http://hz.yonumen.top/gthopouotl.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtfnxvdhvb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtbxarqegt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtiaiocchh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.snrcjt.cn/gtndynplml.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.316326.xyz/gtdlnmmreo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hnxiangtu.top/gtqyyxxrwd.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtywbkkesa.html

[E17] 首字母大写
来源：http://hz.yanxiufei.cn/gtjqhenspl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shangyingyoupin.top/gtqzpyllvd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtrhqgaezq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtbpdlgcah.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtglpfthkh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuxming.cn/gtckqanmqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pengpengdd.cyou/gtkxgzobes.html

Ruby: s.capitalize
来源：http://hz.andypj.xyz/gtyaphjaqm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtwkybohwk.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtthmjciey.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhijiandao.cn/gtndqzfpfq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.9152youxi.cn/gtojxmhkfe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtatuszqnj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtjgawueib.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jianghu66.top/gtzjllorbc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhixingplan.top/gtlukwidpd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtqwmfvwfa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pengpengdd.cyou/gtuykujvwo.html

[E19] 多行文本按行拆分
来源：http://hz.hfpthk.cn/gtjelexeii.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtjltyislm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shzxlz.cn/gtuaesdmye.html

JS:   s.split(/\r?\n/)
来源：http://hz.sxryk.cn/gtumvpwpcn.html

TS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtkgimmoaj.html

Java: s.lines().toList()
来源：http://hz.jinqigufen.top/gtzodlhlnv.html

Go:   strings.Split(s, "\n")
来源：http://hz.hongshengwenyu.top/gtiqiygfmk.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtagfqzmqm.html

C#:   s.Split('\n')
来源：http://hz.sweek.top/gtgpncdujc.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtfsqvugnq.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtapecundt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtmmbyezvz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yangfankeji.com/gthjomrqax.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtiogodqqw.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnqzz.top/gtgyiyjind.html

Go:   if s == "" {}
来源：http://hz.yonumen.top/gtveplmjoa.html

Ruby: if s.empty?
来源：http://hz.iojbl.cn/gtiistdigl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtizctsnnr.html

[E21] 超长截断加省略号
来源：http://hz.jqgufenzy.top/gtsgdbuuiu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sweek.top/gtmrasdtfu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hfpthk.cn/gtobazpbhk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtybkogdyp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtypunpffi.html


<!-- 参考信息 -->