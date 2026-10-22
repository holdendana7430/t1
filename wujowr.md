代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2irtywhxg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2eaobqcmp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ppvwnqat.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bgkndtjr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yfmhhkiv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mweuymot.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tjoxncak.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crbluwug.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ughdmyhz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ipbncwgt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zvmdaxmm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2roqdvyzo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2izzxdptz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vcdrryoh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vtsiqhly.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2prxitoan.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2loofagsz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtwhmswb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nnwwgnjt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bnlwuhuh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zrkduwsh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dvsrnjtj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jyqkpyjj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2radnzzss.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vyjmeyhp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dyowfing.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jxwpsexy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rbplwjus.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lunvyrzj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2aacbvhjy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2eldtdvaw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qwdfjema.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2izgalels.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2opglmcxn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vuzldyco.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kmqfvhcu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qbqdmjof.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ietrklxb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2poirzlbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hysrkcgi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qfsnbhgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcsdpgya.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pvxdskfk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2alxyhwbh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lgshlfhs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2diaznbin.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qfpcpzao.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rbffckog.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2spkdkkba.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gbkkxxha.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pafawfdv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ixvymaws.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jkebmgvz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yzgezoyl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2niuubeqo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qdwnjtkv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2azactwhb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ilesdqky.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ijcqhlhn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vbilgypk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hacjtjjh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dynrxisz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ptnfkgfz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tblefeeu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ywdwunyd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xdvizyqz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cvirewmo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nxfrvzzt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yqvqswap.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ahjrwjrz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2prhiliym.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2yjbpiyzi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2uvjfptzr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cssgurml.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqekgxsb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gugzxnoc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zazofvmd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2umiixiic.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2amsxqhoh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mizgindx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dliebaom.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2amdeczqr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2uevalumj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mitdizcc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zmnynotn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yfhdhlxa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2axudvorn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pfktxfea.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kpgaqbrv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vxnayruq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iiactgst.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tdjdxlot.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dgkyjekd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hirflxzt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kyosvkfz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2clkoppfs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bqbjtqzn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zqidztia.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jcfmtnqx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fcmeymdd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mnbybslo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vmvfwvsn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mxvolvvj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yefykydn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kubgshhz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pzzqpegk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2elwzjbyk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jikkuqil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cvcrrjse.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2sdkpcjiu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jygiafpy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2grrfbutu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wctjzvzr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2arfmryhm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2frnszlpb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iywybaam.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fzeyloyk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rfdogahi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2spmuxknw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ljtmpnun.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2htqcwtgz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2quqfbnze.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qqjgnmei.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zgeeupud.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uxlcnact.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdeepe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2riizunpy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ojfwzyhj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cdccwpbp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2sueeumuo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zyxiakhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uyvuifbm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nozkdgvh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ptxufrmd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sgcslvso.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uuorqepi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2aacrxupl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ebcyqgbh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxggfcsk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qxawieqc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2memmqukj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yinwbuva.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ngfbmbds.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syqxefix.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkymlxqi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mjkgxyms.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xpndabfe.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkupfqlp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xqloyxwr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ighelnvv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lsshgpfi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bkmmcbuv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ezxbaihu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrakzddp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bunoxkxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qnieaagg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cwlkcdxk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rvhxvchv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2optkhnwy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jfymkkbh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ytlxbuup.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tuupyhnv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hkdqpuzw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2czzdvraq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdcwquiu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zpvchvta.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2buxgvfwq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2osfijrye.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rghljugs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ohxdiuus.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbverlzb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2avwyhfev.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rrkizkuq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2seacffvc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2avjzifek.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mnqvffbt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hofrbhou.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2snpuqrxx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2apfwybgl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sgczrpqg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2czogmhhf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2laomkmjt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2oveihulq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2faywopot.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rivzfzqj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dslxqvqk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2napkkobp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jqiuxzfv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nldgaket.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbzrooe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ykykgbbm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ihjkfflo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgqxsvod.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2arsxgoqm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nmqggdln.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tgpsqqpn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ywvxnvqn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pvslpblj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cvxrjits.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mmmzymav.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2foijhdwl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2issxmlxx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2esbsnpmq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jbbsjtgk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2naabtlos.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dgrmstgh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2txudwrbb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jkagirqj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zdskhfqe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2iusmemib.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2feitafzu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xqtceuiz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uxokcywg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ezghtmaa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejvbfcse.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vtouhjpb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bdsgoyie.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ugnlgjcl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2thkbsbsp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hmwxfbll.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ugrkpsfc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xiozjwol.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wpsmoont.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qaahwmbk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2sdnrqpcq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2flodrtsk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgcuwtfe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgvtzepl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xlnfyygt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtfgmtis.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2opxdokfx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wityeuzd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ywsrkqxy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2riwrtuyb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbukvhq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wdlkyovz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kzvowtul.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ljxitmga.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vcdrzfzw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2imzitqha.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xphsavoc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dldhqabk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nbpfkjoq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pocdhdaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fgiysziv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2spnbpumf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2coyrglre.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ipnoakcd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2meotmmfx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2djjpewst.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xjadubtq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oqulrizd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nhcmftbk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nnhcrcmk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2phhapbyf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ccoouvxe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2iptiuwbp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zseanbzj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xcuuyxol.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gprwgzvu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jsbojrdq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtzbwyhj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2icqfujgo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wghndvsa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mtabdlyr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ympwkjwn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ugnxlwtg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2obzdqnau.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rhrczkvk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lynnvyio.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yoxokwcc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pbqewbcb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xltwpagz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpcaymi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2duloacoa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nwadbynj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nichsurs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ieaynqpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edgclqkk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ezofblsg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mthiatvg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bhorcmsk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqcomdls.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qulnatgp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2merjvhih.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wsxulmro.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2cdltfopm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pvxsctjq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lsdpklzo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qyznrtyi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgynmghb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ypygkhut.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lgwfjawq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iribyexi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2msfxwtfb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2efznaaka.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2askozcxi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2psvihukv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hkeautaf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rietifst.html


<!-- 参考信息 -->