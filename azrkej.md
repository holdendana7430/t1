代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtgvwhxyqa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtgyaxznpg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhoulong.xyz/gtzpxvdpwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gtbfrxjluj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtatehmczq.html

Go:   func add(a, b int) int
来源：http://hz.ywan-chungtsiang.top/gttjsswatg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ivvv.top/gtyrkbcsbc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shzxlz.cn/gtefeibgeu.html

[C14] 泛型函数
来源：http://hz.yanxiufei.cn/gteklbuukl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhixingplan.top/gtmugadwzy.html

PHP:  // 无泛型
来源：http://hz.pycfn.com/gtnfmthymw.html

JS:   // 无泛型
来源：http://hz.sweek.top/gtshowpcdn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.kuanghao11.cn/gtlovkjywz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guannengcc.top/gtkxxflcfi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gttuegzhub.html

Ruby: # 无泛型
来源：http://hz.guannengcc.top/gtsarilxom.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fengsongda.top/gtixfmdqij.html

[C15] 解构 / 展开参数
来源：http://hz.ywan-chungtsiang.top/gtsxkexaqi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guowangkeji.top/gthgrvgpiq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gtcpgfdgdq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtspaxbqtq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ehwqpu.com/gtvocxpwxk.html

Java: // 无解构
来源：http://hz.jiagoushi.top/gtbksnmuvf.html

Go:   // 无解构
来源：http://hz.mhx1999.top/gtuwbuhtkf.html

Ruby: a, b = pair
来源：http://hz.hnxiangtu.top/gteedftrkq.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtrawzvdue.html

[C16] 函数 / 方法重载
来源：http://hz.sweek.top/gtihjcegwv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gaohongyu789.top/gtyusgesps.html

PHP:  // 无重载
来源：http://hz.fengsongda.top/gtxueeeest.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ybcxt.top/gtzpfvtprh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ehwqpu.com/gtupsdzvus.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinqigufen.top/gtlhwlpzyh.html

Go:   // 无重载：用不同函数名
来源：http://hz.jlsjyb.cn/gtmtrpokdy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtwocotspj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ivvv.top/gtwjcyrmci.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtfbxmbwsc.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtvaswnozp.html

================================================================================
来源：http://hz.sysykeji.top/gttjagejqk.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtgkuvoasz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinyuanbaomall.cn/gtgshrbbbf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gttfncpubt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnxiangtu.top/gtspoeixoz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shangyingyoupin.top/gtrnpmxmek.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xziqi.cn/gtveklzdoe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gtalvxuhsg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sxryk.cn/gtjcdebimw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gteenoalkd.html

[D02] 追加元素到末尾
来源：http://hz.gogol.net.cn/gtjzllefgz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.quarkkingdee.top/gteopxdhgx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guowangkeji.top/gtatqsfvzm.html

JS:   arr.push(4);
来源：http://hz.cheryme.top/gtpcotidrt.html

TS:   arr.push(4);
来源：http://hz.zycfv.cn/gtxsvwopzu.html

Java: list.add(4);
来源：http://hz.birdmap.top/gtwgbzgcth.html

Go:   arr = append(arr, 4)
来源：http://hz.ydjk.org.cn/gtwhissvij.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daria6918.cn/gtepochtdw.html

C#:   list.Add(4);
来源：http://hz.jyoumei.cn/gtlczdphoh.html

[D03] 在指定位置插入元素
来源：http://hz.daxiang520.top/gtuqxxhclc.html

Py:   arr.insert(0, 0)
来源：http://hz.xuanzx.com/gtnhnodftt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtvoatxwjd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtuyptmzsl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtpgzvitzi.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gtbzhjzhmw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.daxiang520.top/gtdyjyjagi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hysaishi.cn/gtiuujsoyy.html

C#:   list.Insert(0, 0);
来源：http://hz.zhongyouzk.top/gtwtanwkhj.html

[D04] 删除元素
来源：http://hz.tianlin.xyz/gtwaphlsbr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtsxpkikvo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ppjwa.cn/gthbbcizbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangkeji.top/gtxwqpsbbp.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtohfkzflh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zycfv.cn/gtdsyiaxfl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shangyingyoupin.top/gtzoiwlnen.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtkxmrykii.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zycfv.cn/gthepxokwg.html

[D05] 访问与修改元素
来源：http://hz.jqgufenzy.top/gtsutgsigo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtwevebhnb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aizwys.cn/gtyclvwmgy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhoulong.xyz/gtwdtvumak.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gttmmjgscl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aibaodan.cn/gthlhvhnlg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.andypj.xyz/gtunjsiabi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtftxanmwv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtdoxehlbr.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gticbccfan.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gtyjbxxqrt.html

PHP:  count($arr);
来源：http://hz.zycfv.cn/gtpqkcoqkf.html

JS:   arr.length
来源：http://hz.meibo888.top/gtiyivmebd.html

TS:   arr.length
来源：http://hz.ppjwa.cn/gtrjqxwnqw.html

Java: list.size();
来源：http://hz.yj20258.top/gtjryipuhu.html

Go:   len(arr)
来源：http://hz.sufxvd.cn/gtppamknpb.html

Ruby: arr.length; arr.size
来源：http://hz.havefunace.top/gtmykxoarb.html

C#:   list.Count;
来源：http://hz.zhoulong.xyz/gtbzclirrj.html

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gtkwmrivwc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cheryme.top/gtdvkxnjuf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhixingplan.top/gtslotnxke.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtklyfkhel.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtustqsbca.html

Java: list.subList(1, 4);
来源：http://hz.jyoumei.cn/gtsnjmyhba.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtsassgdhf.html

Ruby: arr[1, 3]
来源：http://hz.sweek.top/gtjcbkoycn.html

C#:   list.GetRange(1, 3);
来源：http://hz.gzhubu.top/gtihruzvrt.html

[D08] 合并两个数组
来源：http://hz.cucudq.cn/gtebkumqnc.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhiwuduotai.top/gtrcpomvrp.html

PHP:  array_merge($a, $b);
来源：http://hz.wangdashe.top/gtiuasmlbx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigfzy.top/gtvqnzlbry.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtptmyqumz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yueranfly.top/gtnhjmyacj.html

Go:   append(a, b...)
来源：http://hz.hnqzz.top/gtsberybft.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtewhfjgom.html

C#:   a.Concat(b).ToList()
来源：http://hz.meibo888.top/gtewbdqqih.html

[D09] 排序（升序）
来源：http://hz.jqgufenzy.top/gthqyioboy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtdysbkaao.html

PHP:  sort($arr);
来源：http://hz.ppjwa.cn/gtkkdfquyu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.haohaochexian.top/gtspmvurer.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtmvnsknig.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sufxvd.cn/gtfumxneco.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtpoibrljb.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtyizslenv.html

C#:   list.Sort();
来源：http://hz.9152youxi.cn/gtttxocfkd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cheryme.top/gttgvbwwnf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenjidiqi.icu/gtrvtqmhfa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtkoaswqqh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtzwqinizp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtqafsjlbc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtvhwgmbkb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gaohongyu789.top/gtrgnxkqky.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gtrgzllykx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tian-w.cn/gtivmrzjgq.html

[D11] 反转数组
来源：http://hz.gogol.net.cn/gtbfoyuucl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydjk.org.cn/gtsgulzarf.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtmjblzkgu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigufen.top/gtuslcosfj.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtapekalzp.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtorcsjlux.html

Go:   slices.Reverse(arr)
来源：http://hz.9152youxi.cn/gtvagqmjyi.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtbeplojuc.html

C#:   list.Reverse();
来源：http://hz.tian-w.cn/gtshkzsuua.html

[D12] 查找元素下标
来源：http://hz.birdmap.top/gtbxukqvsa.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtpraztnta.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtiosfurhr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtjgzihxfx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtqduotpkm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.dianchejie.cn/gtmdeqqmac.html

Go:   slices.Index(arr, x)
来源：http://hz.mhx1999.top/gtudqenext.html

Ruby: arr.index(x)
来源：http://hz.chenjidiqi.icu/gtkyonukmv.html

C#:   list.IndexOf(x);
来源：http://hz.jinghuilouyu.cn/gtbcqgskfa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nwbrower.top/gtwimgykep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.aibaodan.cn/gteygpxkmr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tanke756.top/gtixpbkmck.html

JS:   arr.filter(x => x > 3)
来源：http://hz.bjfxy.top/gttschydoh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtvbqswjzl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtfvmjojux.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cucudq.cn/gtdkjewcoi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fengsongda.top/gtbftiuisg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gtqfnjuqqn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jlsjyb.cn/gtttqkzzdk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ppjwa.cn/gtpcpupnci.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tian-w.cn/gtrcwptzmh.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinghuilouyu.cn/gtnwomwzvy.html

TS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtxbpmonjl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtvvkoqjwq.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtjvfnsvsr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtznpkpbmq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhoulong.xyz/gtqfinuvcy.html

[D15] 去重
来源：http://hz.dianchejie.cn/gtpwyerqme.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtkfrhsafu.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangkeji.top/gtxdenfams.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtptnllchd.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtsqkhlutz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hammf.cn/gtadidereh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hywenlv.cn/gtjdpsutlc.html

Ruby: arr.uniq
来源：http://hz.yangfankeji.com/gtsnzwnwdy.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gtzbpjldxs.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gteyjppudf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sufxvd.cn/gtneoondbr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinqigufen.top/gtxecpqrob.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gttjafmzjr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtrczitslu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxinkj.top/gtbgjpajjp.html

Go:   // 手写循环累加
来源：http://hz.shangyingyoupin.top/gtltmvyykr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gttyjrmooa.html

C#:   list.Sum();  list.Average()
来源：http://hz.havefunace.top/gttozlhykq.html

[D17] 最大值与最小值
来源：http://hz.quarkkingdee.top/gtdmfahbog.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtupvdcxld.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtibkaqxam.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daxiang520.top/gtnhlersjg.html

TS:   Math.max(...arr);
来源：http://hz.meibo888.top/gtuvzgyouj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gttjsggmwq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydjk.org.cn/gtqwphlwij.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gtqiahsxly.html

C#:   list.Max();  list.Min()
来源：http://hz.pengpengdd.cyou/gtfkqielod.html

[D18] 扁平化嵌套数组
来源：http://hz.0kj1m.cn/gtxbmnxtwp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fzhhl.top/gtsbqgmunv.html

PHP:  array_merge(...$nested);
来源：http://hz.316326.xyz/gtoptkyhww.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj202588.top/gtmpczzeqd.html

TS:   nested.flat();
来源：http://hz.svipenyu.cn/gtxxyaaxxu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtnazehrhd.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtdvrodgio.html

Ruby: nested.flatten
来源：http://hz.chenjidiqi.icu/gtspimsjss.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258888.top/gtcrkixykv.html

[D19] 按字段分组
来源：http://hz.daxiang520.top/gtsndzcqbw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtfpsbiquo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jyoumei.cn/gtkwrriygx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cashguo.top/gtdtiprdwk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtfddqnnzo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gzhubu.top/gtwqeokche.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gterbozsgq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtqhiugbwy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aizwys.cn/gtkbemrzbe.html

[D20] 统计每个元素出现次数
来源：http://hz.dashuyun.cn/gtqbrikmph.html

Py:   Counter(arr)
来源：http://hz.hongshengwenyu.top/gtxfjukymr.html

PHP:  array_count_values($arr);
来源：http://hz.zhiwuduotai.top/gtgmqelvgw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtupxajtzj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtgovqpriz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gaohongyu789.top/gtspebiqxm.html

Go:   // 手写 map[T]int
来源：http://hz.xuanzx.com/gtrantbjem.html

Ruby: arr.tally
来源：http://hz.iojbl.cn/gtgqbmvuwb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtyqsdcmdf.html

[D21] 判断是否包含某元素
来源：http://hz.daria6918.cn/gtjeuoubfy.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtiwcrrlgv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zdqjudy.top/gtkvllvpdd.html

JS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtmbpxhbgf.html

TS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtfiwemetp.html

Java: list.contains(x)
来源：http://hz.jiagoushi.top/gtpqiqfwpp.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtfxjzagnb.html

Ruby: arr.include?(x)
来源：http://hz.yongpay.top/gtvzzlcpgz.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtfawnbtgm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtlmoxrqoq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gttzsdadzv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gttfrodvjv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yanxiufei.cn/gttigvtlsp.html

TS:   [...arr];
来源：http://hz.snrcjt.cn/gtnhoankiu.html

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtvqziquzm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.birdmap.top/gtibbwdgie.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtcscbyatb.html

C#:   new List<int>(list);
来源：http://hz.snrcjt.cn/gtidykikpj.html

[D23] reduce 累积计算
来源：http://hz.yj20258888.top/gttfgbmtlu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sweek.top/gtxwrwfjpx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hnqzz.top/gtgejvtkif.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtvafqqapt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtigaktdla.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gtyrrnhozs.html

Go:   // 手写循环
来源：http://hz.aibaodan.cn/gtxhsuetxo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtzicaxojg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtlrgktcgw.html

[D24] 字典 / Map 基本操作
来源：http://hz.jiagoushi.top/gtswmtghbl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.redwolf501.top/gtjhdvpqba.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.mhx1999.top/gtyedtqzpj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtaroshnun.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtktotelql.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tianlin.xyz/gtyfeufisa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtapuiwvgt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gotoacloud.top/gtoiqsaina.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangdashe.top/gthewbfotm.html

[D25] Set 集合去重与交并差
来源：http://hz.birdmap.top/gtydodlthl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgfzy.top/gtyhppqnjb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtnkpefgwg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuxming.cn/gtzrgkoxlq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtxplzwyal.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gtqkrpcxyw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenzaomai.com/gtkemtmdpz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gthfzcpdpc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtncwevpyj.html

[D26] 数组转字符串
来源：http://hz.ydzc1.top/gtdtypzkpf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhengqikj.top/gtudlwgdtn.html

PHP:  implode(", ", $arr);
来源：http://hz.wangdashe.top/gtxcijdfow.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtohuyoooi.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtliwkakef.html

Java: String.join(", ", list)
来源：http://hz.shzxlz.cn/gtwhjvvrkw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gaohongyu789.top/gthbukonru.html

Ruby: arr.join(", ")
来源：http://hz.yuxming.cn/gtstcjdmjq.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtutfjrpit.html

================================================================================
来源：http://hz.mhx1999.top/gtkamghfra.html

E. 字符串处理
来源：http://hz.ivvv.top/gtbrnpfwqu.html

================================================================================
来源：http://hz.gogol.net.cn/gtzvsghcoh.html

[E01] 拼接字符串
来源：http://hz.zhengqikj.top/gtifmphkzq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtaumhbsgb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xinyue.icu/gtxdoyxgyp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtckjficgy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtyveoimjs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtuxvfhwcl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnxiangtu.top/gtaoxtoiwn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuxming.cn/gtvwxzghvt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hammf.cn/gtvznigjrk.html

[E02] 重复字符串
来源：http://hz.hysaishi.cn/gtuaqfrmgz.html

Py:   "ab" * 3
来源：http://hz.aizwys.cn/gtlivfitxz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jiagoushi.top/gtjzukxflm.html

JS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtppqwsecb.html

TS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtdwpjucgq.html

Java: "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtwmrpbujj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fzhhl.top/gtqpcyysik.html

Ruby: "ab" * 3
来源：http://hz.hongshengwenyu.top/gtyyopwtbf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sxryk.cn/gtpscuzlyk.html

[E03] 截取子串
来源：http://hz.ehwqpu.com/gtjtrhpwxe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shangyingyoupin.top/gtelzsyzgg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgfzy.top/gtdecoqcaq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangdashe.top/gtzthirwgh.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigfzy.top/gtxvpyzxgt.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gttwxhlote.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gtgdofcjwp.html


<!-- 参考信息 -->