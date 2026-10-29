代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/garcqoflx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gytwnburp.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gaddzztnh.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gtsiytzei.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/guoqhlosu.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gujsqafdi.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/grdactfzx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gzbvocfrt.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gqfsrgvjk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gtfqmflmj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gczalghkk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gurcodzuh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gbwwkfvna.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gwxwrowfu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gykwckedz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdbxhxkou.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gmvghrmet.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geuxwhdpi.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/grmllrckd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gpifvbltf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gpuohbvek.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gryvvcvas.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gtxpapept.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/goljiikep.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gcnipelmi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gnppywatr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gwtaipffj.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gthfzjfei.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gzpxrurdw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gkbvgnppo.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghvuhexrs.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gdtfbqnoc.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gapncaqdw.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/giewbnwdl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gfglpfxpt.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gitayvmmc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/glzhrysaf.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gigbjzaas.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gkycuerrq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/garrusrdo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gjvbuslhl.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/geycrolwk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gmoyndblz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gtuectdqo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gajhyowpn.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/ginvbxoan.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gmlvdrmuk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gslqioadf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gbydggjes.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpybduzqc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gltqetsrc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gmqncsvit.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gpwiiksfq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/ggmtuydvw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwbwxgogf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gamjbwane.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gzsvfofjk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkawesavv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gpfjvatig.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/geprrhhat.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gucdpheor.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gunkiwvaa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/geklqbenx.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/geimwvbor.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggdstvzsc.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gomaooier.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gegbehocf.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gjpntnplg.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/grduecwvl.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gaxfzrybc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gfpglijkg.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gsicizigp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gnqxcbsir.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/ghzihglwg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gpwmvjpei.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gkgsbbgty.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gmhcdjtbh.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmqpmuzfs.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gguzpcpfl.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gcwyfaiuj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gehnfypwu.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gvgkwzzqr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gjainnmeq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gszjquwyh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gtfjehqwk.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gohtixkjt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcvogvfij.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gvhhflrcn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gixizqalg.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gigelkytt.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/giyfollup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/grlzfrdnl.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghbrmakzi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/glqewrlfm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhdschkk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gqrmqhckh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/galspiaql.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gtfstdldt.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gyykplmvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gcbdcxoar.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gjmtmhiwu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gbbyypdod.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gzehunumn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gyyvzmuez.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gyncpenlq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gzlngamjs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gjypneiei.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/grlqxgfry.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gdfbgmuiv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/grgcluxgg.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gsvcsnzxi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gatwninyt.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/ghsgiubaf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gsbvprctz.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfaxnsyll.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwppsydmt.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gcdddsyfe.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gspnuortc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gymockhdp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gsbigakxg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gayfvhiap.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gajrlxzcf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gpkejvuzw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbtddjpxa.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gnfsfulqf.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gcgkoyuph.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/grgrabasq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/grimzrhro.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gyjfpeqmv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gczcqrjqz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ggydfervo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gmvkbsfwh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gvisrkqsi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gloyzzauj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gcgznrqwt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/grcgtxllp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gjucybyxj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/giwrtxeum.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/giscdgjcc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/giruihvkq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvweulafe.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gcwwutcaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtbpyigpz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmcagkbbd.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/grvjvvbdh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gtbxukroh.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/giixajthj.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/ggipplnyd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gszgamcmb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gcchknjne.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gwgwbxdut.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gyfqtlnwm.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gvgvmcogx.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdjldjqck.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gloolkjnn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gbrxgaqub.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gityuowvo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/guolvvyvw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gzelxpstr.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gpjdsmyfd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gxpkkbcmd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/ghhmuoqmc.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gykdwhjli.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gysjeavhl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gipqruoag.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/genpsblvv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gcsdrwikt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gzcmjgqgj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gurvvsktz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gywzdbgwr.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gtepuaenh.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gvregtlga.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gfkicqwjo.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gjmdvanyg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gtcmpvgel.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gapbrfuxt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gleparhmk.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/grdhmoxsm.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gkqyzvqix.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grqtbnbqa.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gqiszlzrg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gfcvejamm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gyddbbnga.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/grghndoka.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gygugxxif.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/ghcemlmye.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gqjmfftnx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gkbdfeudj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gappyujqh.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/grjpdkrtk.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gezfkqcfa.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsivyqynl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gnkgetkdp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gnxpsgpsp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/goosnjqcs.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gzcuwumdr.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gpzjhbkkw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gncnkwldq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gnjdkjpec.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/glnchcvat.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gppjwmidr.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gsfoujrcu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gohumhayf.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gyynrisca.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gtlekpnix.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gvcboklsp.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/ghobfkgpy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gzdffbeyn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gsljjuusz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gbdkwxkyj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gdakpspid.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gbtmkziog.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gzsxojvyk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gduqrwhna.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gdcqoeifs.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gmmfhovqk.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gsimhcahv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/grvfrgoyq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/ggctfdjxk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gstouscke.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwocwxcb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gtgnsbhre.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gtvttvhuj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gtvsyzdhq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/ggocqjctj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbyupnlyw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gvbjiqmod.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/ggvzulryf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/glylscoxh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gswyakfmi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/golawuvha.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gsxquynzg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gwkhzzakh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gljubruku.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gannygskg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gjgilyevm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gjzqihffs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gobuaqmqe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/giavezfew.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gslvrjmfh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ghalyphxh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gcovrnbvp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqomgzcmg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsfyrlqte.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzfzqbbhi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/ghvrbzadm.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gwtehbrjn.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/ghtyekkva.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/giffkomtr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gepxnbtev.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggysqujif.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/ghyjaagmb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gktagtmsj.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/ggdnqapfg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvspbgdin.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gfxzjhged.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/geshzdgyr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gklikrjvt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gyenkgvph.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gboyotixc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gktgkuddl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/ggxtvgjkd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gqrwzafis.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnzmkeeqe.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/ghsgiaddi.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/glvhzhqkb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/ggbsftqwc.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gexeiiogq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gfahiqstu.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gmndglmmk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gupabwnwj.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjewxkgui.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/grvmyvame.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/giktvjbky.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gldemknyf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gglvrpiab.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gsckziqhi.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gcquncegp.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ghoejcsgz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gjamfrppv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/guampikqu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gxoftnfcw.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gplpjhult.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gazxcxvvh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gpnlaiytp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gmzdexkcf.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gnrvcpmxn.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gbnxqxjon.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gmyuribmg.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gbrkromaf.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gwfzoltmn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gncntbwat.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gmeokmidc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gwscvfwag.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gpfirdsoy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gjgnprbde.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/greedpwxo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gsowhemex.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwttllcly.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghtjwtyeg.sHtML


<!-- 参考信息 -->