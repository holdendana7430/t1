代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kvtyxkmv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hejjfbfb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gnjrivkb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ljlnkjlv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gncqnpeg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2amgrfnum.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2awuhwlwi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hlspaozk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zlapvsys.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvmqnkqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2scwpltgn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzaeujet.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nitgilyv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2eytdtfcf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dcymupde.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sekhscta.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uoovbskm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2psxjfwbm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lmsgncjy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rmhznuuf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdlyrknf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciqezxzo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dpizwyww.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vzmzaapy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ajbpxomc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2welsxvvf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vqcefabk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2peqpisce.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zicythja.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lacnnzop.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hpxvyofn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jfokongg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kfznxvzy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2sgkgnjcb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lzxxmucl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dfscmwhc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cnsdggby.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2spqusyap.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2toqacwzo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qfydzcyr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gvvmctnt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zcuzcnkw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hbvdutxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pblunzng.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qggjfpnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qctfcvbz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mlqaswlp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ipgrojgk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2civaskyb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gojaphmf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pdnlhqxd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zlaaxgag.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sosmtktl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yrpocluj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kfnfmwdz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hndpzptk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xhfsgtkx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jafqyong.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nuqrgzsq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gagflgnb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ccxmeuak.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nuokwnoe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yjjxpwuu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zkmqiaxp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hpgnbdjm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jnzmilxw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2aprcbdit.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tzdmfkoh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fiiyhcyv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pilmmvot.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhluoxz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wgchagqi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2keftqpcd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ttbqrlfp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dpotftge.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pyglmdpp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nzjonnes.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hymxjapu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2grspogyv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zicfqbpp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qpglydgn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jcwguakq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzbhrahm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vpbamucx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2worqqlrv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hsllkury.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cwwgbuta.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fvvxhhjx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2umjftgtg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ssgzukhd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xjbrmnxl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hrznvqfn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzjfptt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2thelbzdd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bsuxfrze.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hzxjaovx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rktliefj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hrfrdhkb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2baxbfryp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ifnpsbin.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ncfdjaav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rnzieyzx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2onpukqww.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cewvbljj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bqvkrvbd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xewjzqps.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vfmnpohm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tortipxz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vqwihtor.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2majlseuu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yipbaekd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2erstuipl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2szqoohfd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2raomyecl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rmqasjgh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2aifkgzoz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rolbtxwu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tivdpduy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zdzbqbxl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pgqsjcdw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iowfjuuw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qwakootq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fqgrhotl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wmnluofa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tknrrnff.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ptnmnmsz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pbgqbzrb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2byguswpk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ivjuznrh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pddicnrc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wqgdctom.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tpniwubt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2maxtmjfz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2aeeceibn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kyhrolht.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vgfugubm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hyqdtyku.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ewvwrcow.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2dvhpowux.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rretmxgh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aiaoxnyz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ywjxnqnf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2azpinhcm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ludftpmv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hlrcvkoe.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ihnjbtgc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kwzhgvcf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhjwxugf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2edftkxyr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hkotufor.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2srnasvcx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbbxlrxk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gwmehttg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jneujwtm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rkpclrwq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2obkmyvyv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yplmmgvs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wmfqrano.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bsflusrr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pfsnwsaa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fqjcpqji.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dskxcrye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cqmbeorf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gtwueznq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ucwuaror.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cgpislzf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lxhdxbfk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mcfgknjc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2opuydowo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gglhwgmg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hvtwwamw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fjmpqnjk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tiumygxr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nfetzvsv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbjfqzsh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fneqqkiq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kgbigcft.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fkputxac.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xwzouiqw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hmircahy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrzfbvyw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2alzyafxa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2onquecju.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vwpqtqfg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pippnqkz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zumoqixc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mfnhzmdy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2utwoljqt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ohoydeyu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2druvaala.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ojjiitze.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfponkp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjfmwcsl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkhhtzgs.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krrbvpnq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2atxzociu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zimlardf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gkgolpgp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gxyqfxug.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ofdvnmly.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ybwqtzkb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yrjfmhgg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fojkytqk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hkqsixpf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xqlafbjz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2acpgsrhh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dcktzjmj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwzaosda.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hhhryaki.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hafvlcqw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vaqvxfqu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ksasfbdk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vpgophzr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jtqhprnd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jzvjjyuv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hkiucdhg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rkvywjwd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nrzqcrzz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtwmqdq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itpujsqm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xgqptxdx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tjzqzxhh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ztnaxcnb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gdtnoqmt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2megnsfgz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2trmmxixj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gekdyzsd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jcdsyhkj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ysaxksko.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etqvnxpc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otejskup.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ggisqqrp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bhrpuyes.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2diubbitz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whzznrmo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mqgotnqt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2oxfzlfge.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uiwzkgfh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zikrehor.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tzfcbphp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vmycsyzw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qyhjmdlj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wzmidasn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qoppeqey.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zszyexou.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2uvnhfvwr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2crnvofvf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dyphqgrs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mukvbqna.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qwskhxil.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bfzltoqu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2csblsmsv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rzlxzzto.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2frnbmvtv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dxrvfcts.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2plrpxzrc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lfnfrlzk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qxpbizys.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yjjfxrks.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kaxbzpkz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jchzqcmv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ajyfijfr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2blfxogyy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lddlwydy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qttqbvdb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zzplhucz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xuixkqfi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qizyjwql.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ibsplosi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2cphisuwq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nmvtveym.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2apugpppj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zymjzfyp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qpnqrvbk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dzbzxbyy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fexrwpos.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zfsllyxl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ccqhjiuq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xvqjiagp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dvvzbvpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owsmmgfm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qjoyqsfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouxigxca.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nxenksoe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2seeezxnm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bojbvxot.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwkvkmg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ztzfifxz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dgyfpxyd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wxubnntg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xkfywnwe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozdmukji.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqllcbii.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2secmfbqn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgmkrkql.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2endfaboq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nrvybzoy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lvrtoxtg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpuyybmr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vahrofei.html


<!-- 参考信息 -->