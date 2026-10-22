代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nfwevifl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hzkwayfx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2olicmjqy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sdhnqcvq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmlfeqhe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hevpitcg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kugwthzi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lvilmjmj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2atogvbjz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qqruvfiw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rqcyixiy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ecrkqwig.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqszyesb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fmdypgvq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lhqlzist.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nxexjzdm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rlpkkdan.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ztwdtrdm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lhkguyoo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pesdptym.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rwrvatfn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zfrvhyov.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lvuzjryx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drdwsnmq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vvgmgwas.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mzxlrmac.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vozipfwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwsjgosi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xzuokbwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xndjxkxj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yfsewyis.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gwymnena.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sdprpoan.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ieusmxfy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sdihfuwc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zuxqvksi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2yyqfosrp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hwcitjua.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fkfmtexn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pyhqmbwg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gbccohrj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hxeofaid.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qzgnlsdn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pbpzhcps.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zufmjbij.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zwpykuho.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2axxcjygw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nlrlxppg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vdepoqov.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2raxkahig.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnohomng.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2bewayayl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2htkvudhe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2utqntcqy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xvusqbbq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mqpcbnyz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gondcfeq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bdvpqgub.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2epzaamoc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tuqparzn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lnisaude.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ipypmdpb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kkjhlyvz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2onwwpqaq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zjqbbpln.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ifcrpwzq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iwrfndke.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mpikmwqy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uzpbdecx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2duesvaaq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ttdiouzq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yxjxdbns.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rdtvonlh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jyikhwrp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hdllzovt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nonyptxs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmvwyss.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czqejrqx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nwvaechj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nccltqoc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bltvxuyx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aichblik.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rtccpbum.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gyxnbwbf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vwxsuzms.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2clphwtco.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2badfhain.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2posjedbn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jssbvcuw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ekdadtjo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2aghubxoj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ipullbvo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xiwxreif.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dmrqxsrd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xrcqrqae.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wtxfiluj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2egudhyoy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dapbleau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vbiplwgd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wtfweybr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qmqrsfkj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwdxdlaf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ksylisuo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ojzasjya.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ljrfjwfn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ymgzijtb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ifyqwzbd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ulpfmlqq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdlexido.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bzfukqjs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2owsultzi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2acnzxojw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2koxfaqhn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2thnptqqm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fazycnby.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aujbwzil.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2luwniaxf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2pwyzidwj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ixbpbmil.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sixdoesx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cbrhbvlp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2asznblfx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2szqlwefj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oqvtnryi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fbwmmmmi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cfubmeyu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2bszsuhbl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2swvcxbjf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hlnhudxm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ocecfntc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nirzhprg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pbhysten.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uxgfxtyt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zbiazjfj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ktrjkdrj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2flqexhnl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hoqwbizw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wegdlqdo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2inspftod.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rijnmjvg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bmgdjjdt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jfcjjrzb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrcknlq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2thkkfllf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ilbljmlz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hbxvibwd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrefkfgj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rktfdojv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nemlznkq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dauafujp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nairmfxu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akovpfwl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2svarwhwu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyiekpep.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xeoqgcaz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2citdgmvr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mesosbab.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yioumldm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2mdnjncfs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ccelyehv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hhpekfob.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nxoxradu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2frzzixog.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zdwbvtvh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ohpzfjpp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hmvrffsi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbgcmetw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2glnccewx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdzrehx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvfmncxs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2evipucnp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2omnautmr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xkvjlayh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lciyfjsc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yumgvukx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2inyojver.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vapkwxqc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hwklsgxc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wjqpbbai.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gbtwwwqx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jssfalcs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2stgdwkti.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ggodgjpq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tcympxka.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dkfleajc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pzilhtem.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2uluiiwuh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2izpohbzg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xipmrahh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bzmtpkvg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qvmsmlyn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kefbicau.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pkhraazl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2guuqjgvk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fisflxpa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2betjokbr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ujkwhfhc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ihvycrcl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2eywyrnzf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2glmktxpc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ikvyijhk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mdwqwauw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2znjslqeg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdgglnrl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2duajnnaq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2khipajdo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xebbnjeg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2keczdhsx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xrtioslg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yhwcqkua.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jcjqpntb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2htlvhzje.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2labwgttp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bqskfdan.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vdnugbak.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulplvmob.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vdtxdxfm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cspyxyzy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wtdmwfou.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lxcpemwm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vknlkixn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hfawtgtt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsakiylv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dlaonvhb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wjudwqyj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pdcgxudk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gfjruwzp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lsqoptev.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2inifxoyi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vbilqtdx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zkcmfihy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psmllvcs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pljywapg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2swwfgdll.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aqfyjrzx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ardmptwn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwhmiqc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fhmgiytn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yalwtofb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2updoroyj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fgkdsbut.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jwybixgr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bzkaycpq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gkckttgl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2daspxksg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gvnaemuq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kimdqppq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2alpdvapz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mmetmsef.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vskdueae.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xzqfdced.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqkmivj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hbxfskeo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xxkzidts.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tuseaecy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bkterppe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lpwsursq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmjkmjht.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ukfwmmwm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bcnpulwo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rbduaaou.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uyxqkucb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yszrleju.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2izxcjerm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sizbwjya.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ckeozcfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhoxeqkk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2comdqred.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2twyjtxut.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bapkiffj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cdrftzjt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nnppqowi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tgxrwvki.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2byjgntrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2razmgfdl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2asqjuxov.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ldgqlvjr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kromhvuo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rocxlxwm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cwvxfyul.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwygzth.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sufvcpbn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2myehrqkc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tjocygtv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2irqoktzr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jdazzlpq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xyunwrab.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hkatfqqf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2udakjxpz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ezhakigj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xxrzcdan.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wzxcqfel.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ycyyvpov.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgyffcm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ijcschgm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2imrndfax.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bczvouhj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lgfvjvzj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dhcobofc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2frricumy.html


<!-- 参考信息 -->