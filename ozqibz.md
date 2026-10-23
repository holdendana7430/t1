代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tcnyaahf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3hvtfcabm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wridojfj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ycvqnkuq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3oaqngbdy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uwapwxdt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zybwpiiu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3eecvnumi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nmsfolcg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3eovzqakg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjidtdna.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vtroudwi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uyankwxe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkwdqbdv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bbfxbqvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruyaqyqo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3htmxsiwl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3euojcybn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xidoiqzg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fsssarah.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3shsnmyzx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ynzajudy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ggrrhxtn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kvuietua.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxquqwwo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ljczhxbm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cihppsuh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nxxqpfsa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pzwbroar.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cmnzrwij.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dskdcfjb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dzljfbfi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mgylgids.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mogpnqfn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3okygddnl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qkufaolz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wthmnxqy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3onxmwcdn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ykdqqmfd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rxyhklva.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vovcdzio.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pywqdkmv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nglhcidd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmyvpich.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gdbexnxy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kcgyuxsx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wguwpkei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcpqpjwv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bdvdsnct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohsasuuo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vplyiflq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eskwepsa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lfrfyhcc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pcaumppg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3aegkfgll.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lqufghui.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3atnrvqlq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oeuzhdhx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nonuodia.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gexbkzwk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kgmelajs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bvnbjuvx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gpnxkdpg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wwxlkzsr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dppsvdqs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nqclkxop.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mwekgjln.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jexzjnew.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lgbzteim.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qhvrrkru.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pbknbbyz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3konxslkj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mxwncqtc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ughofrxs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lmtuekem.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxcbcbb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qsnzbhdn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sduyemxg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rttffgdx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdcyofhf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3awqsladz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pksarwxq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dzhnofly.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3futvpmrf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3waywknik.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qhlfubus.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fxglpwuc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qfpkyaiz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hloqgxtu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gvbttdqw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3yjotkiaf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vcdkqryx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yrqfnfea.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lqqnbcqa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rvaqtzyi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bilzagjy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zzcwsmxw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnqropnc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eagjejcy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kpmtfrfw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3akuaurwr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qnjaibfe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lorygyxn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3npkierap.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tlcxiyjc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3baulsfrh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wfrwfzun.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3culqtclk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ptacrxlm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oqbzlepa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fyqitnwn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rhgylrnw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oilfvmig.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tynmxvwi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hmpojybv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dqjccwyt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xgutbbrr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ywgfhodi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jsgzwymx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ypiskhrl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3twnohqua.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qbypjwsg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bsyzjrme.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3efzhbfyt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lzyqlnna.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rbbyszwl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3krprpuek.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xaercdzk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ocypbxno.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ooamnwml.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pjmsszmh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kyiyhnzp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hvrmdsxc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qfvsymfx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpojfoj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dzajeove.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gbhpkvex.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sqdhwdlw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3oowsapnp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3icgsrwhc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3paqbmypb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iytbkyzq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uqpuvyqg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zknjrfzt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3aencptac.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xbvnkwgn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wsdlipbd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lqqaqwav.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xsjbtlae.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3whsayzqn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3plhuqagu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lnbngvlt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xkwqoves.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3thveadnl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pymniijp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rvsdpaca.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3swquebcw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ugpyhofr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dprtmzzx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3djipcvyp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vbxojwyo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhnvvjc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3anqzjtvj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3baaawugp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3snrgnnrk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rksyjkzh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3moxpahgu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3udyzjogd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sgkmugns.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kejeoifr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amhtdwiz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vykbxqzw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vvatyvgz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekmwwsuu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3avpaeasy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ikhyjvyc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3syalwkvk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wcfgabcz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcqcmxkd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bflwnmxx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hoodygvv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jnspdayz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wauqgauz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3aadvsfiv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dkkiacle.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lgzulsoh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvcarrkh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3exsajxsa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mswufzqo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bjewmajl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gblrqzav.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3diliviwq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qsmpyfwo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vulxaraj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lozuczkf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgyinrmo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vhcypndl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdeqrjo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wuidynhj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ydjbgktp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbfjgxd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ankmxira.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jffdabku.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3amysphpc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qdqllkfp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3niijnytq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3yvzyhpik.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fysjvksu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ktgllepi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ljupgfcx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gzdnbwqj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3umcxlacz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3arvcyfyc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shplyjzn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ckwrccno.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rswvzcig.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fnpsbchd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cahoedjr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qfuawpff.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kxqctmdk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3liewojyd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dedwcjvl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3afjacbra.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3scmgvuxg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nlumdkfl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nmrlmkoo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3awizatqt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vvjbslfv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ifkltani.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ncvoanqh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3njketdwx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3seivqdze.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jbhtzndf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3srurxmdz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uxtajmev.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mbyvxzqb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrhcitlt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3erhxowol.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arjtvkuf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3eyoaevlo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3iestqlhi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3emgedrnn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dljgdpxv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3leuovvol.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3sqygakmt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxkkddu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3cbfujewa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3azqqarzi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tdwzdgki.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ywpajkdd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eoacodpe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3refenlra.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qnqjghum.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mvneflez.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzvezrxd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jsmmftuc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqnrmnto.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3oylbitap.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pdedpnwx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3igkcluef.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrbhncm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ubrfzglk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gkpvpdgv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ytoaeggs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uhemtzza.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jnaaybjw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3apjxxvef.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hstzxyay.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mrordbqh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubsvjcaa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3veudskln.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3byiwkbrk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fkzsfixg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3awrtzufs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jbgeqbvk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oceiqyjn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3frmbdtoc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmttxpub.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jdbvndtq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zmhpqrvd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cllavlxj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bjljwxso.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fblkqtuc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kvztbtzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyetlmar.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rshioakv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmqlgwug.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qbdzcgla.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jcfgysay.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3icsctpvk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ansxkbcd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xcycniry.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ggarcswg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ipkvnozf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zkcudsld.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hyfinehx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lbzyzaxw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3flmnrebe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ilkckqvv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zkfvpyjy.html


<!-- 参考信息 -->