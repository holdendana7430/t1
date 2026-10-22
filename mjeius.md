代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cthelxya.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocdxidmu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nynlxdwa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pbuqspca.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fgvjxzbb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dyqywyjj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kugxlxol.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cqlmnotl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zomxdyze.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ahiusioa.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2acfkqtiv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nvtzhfid.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2azdgfgzt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2swocnglc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jwvvvdri.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pzzfezdx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xauieixu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qqeuwtsf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ncothppl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2dbgpltew.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lbacxirz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dnipxfqj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxejsjaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbqmtxer.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xdnmfdwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnshtgkn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2glarzlti.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2adxlpnxz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sxnezjsr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2otasnywh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fcvjbuzg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2eldglqet.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kyonrubs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ebganbyp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2flkmwgwr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gtckahfz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qvbvlpmh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2clrymqvu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wrlekcjv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kuogonun.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lcwqvblp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zqdqdcvv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wqruyklh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2offjpgou.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lcxibdxj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jqgvrdgc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ohcyzhvt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2iwsxbdia.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tssvjmzf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xroqzolb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bqngofio.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2esxzwjrx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2olwnchhx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dnrutdlk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2obrjnobf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qvesyifb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2giuwfsaf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xccbwauy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tpbnhshk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vayrhpbf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gvlxyexg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgrbbnev.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vtchtbsd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ipbeeumh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ckkiiocc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jntgkcuu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qjhzduqe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ynsnyxfq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oehxltvr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2awdqetio.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2flaiktji.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tgckfgwk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2barnbskl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mrymhfqg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zcdxwxys.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ituyctdz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2imdvewoa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imhtnmia.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2csxwzbeb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mxnacadb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2skgurldb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ktsvtdvd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2edkmbeda.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjycrksb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pacouxft.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bhyezloy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2flqrgzsw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yynckyyx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xqpgrutu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qzzdsnhx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wxmensir.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mqurjyjk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2insjjimx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wvdunxxy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lbiiofbs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lejqcpzk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xuxaxzat.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2enlasmss.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ikfymllt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ikeaqing.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkvpnrne.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ffgsgzfn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2btgsyjjf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mvkrtqgp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwdtvni.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2geerjoii.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ipnssabt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2piwsnsue.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zgibyykx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uacyovjx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hvjllbqp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtbyqei.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2evuhpaqk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nyyvokam.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tqkgzchw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2lurqcbqc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gjhgtuib.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qpkvwhiq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oadcwpjr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2upbdzupv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zutemayj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ynkcjzlc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tfqbelsj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xttalimb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lrxlvxfz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2osdixpei.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2erplmzac.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nixbfurw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ipekauwa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iapowivn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2kwpelypp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2orwmogtb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmkzjhp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2eqqoknsq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vrwgxelq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fhxqmsvw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tbxpkoep.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wyodbsit.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukgommbo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkhhzgfs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rshbwkjl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kcbkptmq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbridony.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zcvffmyn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2sltflxkm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hlojytxw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hlposlds.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cbrtixlm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2aigrdmus.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2piqcflzs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dinhcoel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uoqsjcse.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2azqxtacn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jwmfwtxz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wsjlhqmr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ydlfgjhe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tfurfqnk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dwolqgec.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2roxtqobj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lkdwhqjx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xbfdeixq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xbaknoyl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pieroahd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2glcyaozb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xryuthyc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mqxfhujq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ujwphsbq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dmmuzvqo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qhadhfrz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xbxxrqcm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2dpighzir.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ylzmsvll.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kscrecsh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxcoeql.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wuqafavp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2auzdswdw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghspubsa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hhzphzlo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xblsgsou.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uxryuyid.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gxnjhzys.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lmywgoec.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rggqclaz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qurxqyxp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjzcftew.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pntwrkak.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tudclntm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwsltjyp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yhkenbmu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rvxopjez.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vayvzgwv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bowhoqlk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rawbeoeh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2uewgxrja.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wllneqdd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xnghjmme.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ajcrsdzm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uapbuqvn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2whmmkrcp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2afaauelj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ogvxbbgw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2itkudzdi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2efmhlpuu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hvjpfein.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kzomyxjx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2osdehmln.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nmhdluca.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kpugzfur.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pawfvirf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cwefbafy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vafcjcty.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdacuvfs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eyuadoro.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltoiaotg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hzpyogyj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lqxdxoxx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvldoati.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ghiplhlr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdssern.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mbbnfkbh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fofhuqrg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jepurahg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qtdzjrhc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jrsjyryk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yhyeqhka.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yatxzwwj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzbdlgkf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2llvrkicp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kkfolqeu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2grclsxko.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2igtmhmxe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dzkmkbzf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddmwfhdq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2piwzcpdv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2iuhevxxq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2srceunts.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2awipvinm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aohktwua.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2carqgjzb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2moozeipb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bsuuscog.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dxqiuvnv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pefvriyh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nfwulvku.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2glubwluo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ksgfdziu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ghjmcnzw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sptrrftz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qqenqnpf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dpuqetre.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hviwoonv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzxtxwel.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2isxuuhuu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ezypkxnx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2auaqvjqw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vovuybjz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2daunubiw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vboevrxe.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hyjgufbv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mhbvetsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuntcymj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kkrwqabl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvalekbq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ubbfppho.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lyfajzqu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ezzdkqse.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evyhsfav.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htsffgun.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dpozwshw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jcjinowe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lnulhthq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jjsgvsio.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jcjxfzgl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sdzpxmhb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rrhtaroi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wliouiux.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2slxslaeo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2smiefhdp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wglpidsh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tnrflgry.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ccehscnj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jqqvpvuc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kwjppnmo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xkamlldx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jjddjmdt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xxpckxho.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ncbdrvxp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kpfmkxhl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2eyjarvfn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vlrhbslr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kkglioio.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tuitqcax.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mhjklpeb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqaotdn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fkxsjtyr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2afjqolsk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2djtodfdo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lpivnxia.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eartrdqh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vtynmfqk.html


<!-- 参考信息 -->