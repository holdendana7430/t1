代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2isybzenm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzjpjcrx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mribqtoh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cqwfdsey.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqhxfftc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zqzacygp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nycvpulr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rtkvqaus.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgfbnmrw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2sgbgzpie.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xweanmfq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ntwmfsdy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjuugohe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tbqpxywa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ayzhqvse.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ogxxyinw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ewlgpftn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xriueamt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mpbvvnko.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qxyfsxls.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qntraefv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cwkcjckw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2woxqxcio.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sazweizk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vmvhnkal.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vagehpfd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rnbboeqa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xhtxxbim.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mprdbuze.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xkorylzf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2aawnbbwn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2oyunfmrb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2fjsplfbb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2scpemhkb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ariaxoek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbizkewv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2apajmojh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbjvlqmt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gpmplblx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zuwaqfep.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2excbvgmk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2igyrhutu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pclqfiuy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2menimkpm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2etlobskf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ulveuvgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hjdiyesc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xjqxqcsf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2enymsilk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ytbwijcs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zjmiuqix.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2haqyfepb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2noetryeo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ywbopnry.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ehwzkujr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2oakpvohk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2owbsnqlt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mylasbyx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rgivkbou.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2eglxgwcx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xzzzovnf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gjqkrytj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rkquvxpv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2evjgujtf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yurpdqbv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mffdxdhp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2goixlafl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2scqwkswb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hxsuxbbv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2heoserzw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ncakoqcg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sjmdqcio.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2outmmcll.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mgeklkgh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2okldahek.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qzdeculi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2friylyyn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pbedcfgt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tcvtbjcn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2abettdfp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qfcnmxqo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fwcapsvz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kjrzikvi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fnhmskpe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewdznnmf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmlxvefm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xcbmsbri.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gndecqfz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gzxiutdz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nerasodl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vzjlmsvu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ypvmauhm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xirgtefs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ubmemyaa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gcryulex.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dpbiljzt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ziapszao.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xyoblbko.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2npannzab.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fdgezznh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nuefqyts.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ugtjdjfd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ibwfyftp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ykolyzei.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jupdqynb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qfcgueaz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nqbjrafn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hotjhggs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2djycfoky.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnqlistw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wcjaetdb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pzmxdgrn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dmgvdrpb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2noxghxwy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wsivhhmt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2sdsclpdp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mjxchmxl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nnpojrdc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ldzexucq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2begwlcmq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dbwczcqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jcvqxikn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jdmftqtm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cyptbchj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lukcnxlm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wbqrcrqn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hqdzlpkm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xdiiqtok.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yuxtyjie.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rzkkfqnv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2synjzqvv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2glsfjetw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xqjtikid.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lxsvlzgm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ubhezyes.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wvodapbr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2acmlottz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bfhctfzq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gyelxyqp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yoxpewyt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2okgdfqxx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrhfblkb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2yvspisgs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bjzydllj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2pmplsqfi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rliywurj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2avelgosd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iudzizem.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jcfnycfw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lqmfvnpn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ghpynvgg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xwqljagu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gbbljqpv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2klmcjmjo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yedeimoq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vgbacscf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hbmemhbm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uhbwkswe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mnbymcok.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ybtuusqd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vronmhqx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oyihbbid.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mwmpjftc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xjwzqmve.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xbqktjus.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dfpcdwql.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkbgyjnd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nrkxhzeu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fcndquyo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mkbofjgv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qeziujyx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dorkmqtv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qoxgdzue.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bcpkbrgy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2esunijss.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2stuprpdi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xrphsxsu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2raoelpsc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bznswtni.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cvakezvl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2srjzvhji.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2eakhbllw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iumdzlqj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dawrfimm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mfwpmkbq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imwqqedc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pzirsycd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hepxjnse.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ksvyevvb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2exbkagjr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gegirwof.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ypqjuokw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mkhfwvtf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2sbmvmbrt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tpaijylm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nrnvjets.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iddvbnsm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2anpbsgqh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nihtjvgd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rxjddvqo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xhnvbeer.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ylockick.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dvawsydy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2izrulhpy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uvghurov.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gdmfdzdq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cizxpbnl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2outctzjh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2niscqfnr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zgarmhbc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2holoqidw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2elqowlvj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2asqqqytp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pbfbxpkj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dirqxrmr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2biaeixvu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nmwnzmyh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lxaurlzs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ycreebnh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hcapstpk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wyyasleo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2excjsrit.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbloshsj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pfbmjgmu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jytdlibv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2schbputz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mindnego.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zywrbzxa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgmoeczg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mujoghvh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2onaiafbk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cjngvrzo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wvkzfrwj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mxxznyjf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mqvwslia.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ndgdrqnv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2oanlqvqm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aymvnzgp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nlolfuuz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iybknsuh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2phribxcb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2afmofgfd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tourteir.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zajhqxqu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nxhzttof.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ajyqsign.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cctzcxsu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xccfyrtl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2meqpcpeo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hqjefeoo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jrqesvmg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2meqoqwuy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2diufrgcd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2fmfcpsbx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2crbtjxpp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nyvbpqts.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zjqdvcud.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fnblnfer.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bwrnrtdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnjtfuy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pfnruxnz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwlqphwt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zfxeeaqb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2godnhkww.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mgewrzjb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rfulcpdl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wvmccbvu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ftffyxzk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gwszrbcl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zorfkidx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wjfwpfkp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dkgdkeeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbebwswu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rqvqaqvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2optookef.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igywroth.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lfgxgbny.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pemlsvse.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yuashpjo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ufhfybwh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ifecrlac.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2svfkofvs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2iqochcor.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2momolvwx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ehlhefvt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2empkkwxx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zoobuvbb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rbmintsm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ocfxbvmy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ojwbeeva.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zsykokgo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tldxjogd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ptpmvntt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2raiduoue.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ewvsrpfh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ypzxqfgd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2udgjdpfl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ozjpkqyq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bdvejntu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bkidoatb.html


<!-- 参考信息 -->