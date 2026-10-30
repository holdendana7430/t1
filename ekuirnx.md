代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gewydpznj.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gnpoibybu.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gkntycswv.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gouwzgugs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gozurkdzm.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gmptwshxe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gwyeilznm.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/ggutijvmi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gmtwymyey.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gfutjaeqz.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gpksgbbeh.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gjrrwnyyd.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gymniojqe.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gkeziwmbj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gnfengjtw.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gcvqrhnrq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gkifwsczu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gmxtnkovl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gznvahbnm.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gvmzyxudn.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ggiuhwpeh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gibhpkvfy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/geentimql.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gilsazwkm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gjeqbiyos.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpydcdlyt.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/giuhhkmvx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggluhloff.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/galunksgh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjuwxyjzc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gmkmvbuxl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkcvxoefv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gsnmzfsdo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnzukyvnp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmcbhkogf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/grkjokoov.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggwkterkx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gxzwktuvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/giibguuin.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gghgfrfsc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gdfuexnnz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gavfhoksz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gvvjmastc.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gcpazlkir.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gzfcfterk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gxyosjzea.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gviovnblj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gtxvdosnw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gwxagfcpo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gjrpobacc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gglztfhsq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gxdkvocum.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gurtxvovx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gfolxzyym.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gczayvhcj.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gzpludchc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gojvyumca.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gtykqssyh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzlpcpalf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gryurhftn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gbfgwwbsx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/glopvvoed.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gokgfchjq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gggursfpn.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/geqjndedh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gzjxobeop.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzswszu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxgoqbzlb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gyapsycty.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gzmhizfys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gqrlzbscr.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gypbksioy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/grhxzbnxl.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gjviiysae.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/grsxxavdq.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gpixpwuwx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gduhmbqnc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/geiwebwpw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gjksrcsqi.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gauhqlhkm.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/ghlkzfdkc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gnmsiujga.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gaacjbxhg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gjsiqdiae.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/geghsviyo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/glzwjkmxj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gphsovtdk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqmnilf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gkuheeani.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gcbufetnj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gfkajrbdt.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gdkimwyzu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzneyfbs.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gcqalhzef.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmqutbqgx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggtwazdpb.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gpyjfsiuj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqppwjoox.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/guieezpnd.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpxbrmaly.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gltwhlgek.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ghgghyshn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/grmmeypvv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwzjhrpzq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gzvflhqed.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gczeqrxkp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gzxqkwosn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcbcqaxbd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gjxwvitxs.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/ggnwbciol.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/ggtmkczrx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gohdamtmw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gvqhloyre.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gcifynimw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/ghponvmth.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gqmsvqrgs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gnsolxqvc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gdkbfadzg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnkovuetj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gwozgdrpc.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gifhckhuz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gyinenxfv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gvnznxbhr.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gsrjqiyog.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gzcepeqbz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gmoyqeaaz.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gggmdbdbw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/ghesccngg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gwmgufhrw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gogpwxfqv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gxnayytxk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gbwrfabky.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gwabtyjqm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/geonfvphb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gquegzvru.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gelcapkyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmjubepok.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gintnlgej.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goldtmryh.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gdmclainf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gwhaabmlx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gzkrdipyu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/guyxcmawt.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gorokfksm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/glcqpxpdz.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gkkfvkrzc.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gqbsfixwx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gretxhmvm.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gnhdgdapw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gvwxbtyee.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gpzttuxxo.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gehrqoyyb.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gtudxdpya.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gvoxdtpib.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/ghwyvopkn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gpmjgmwav.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gyqglrxhd.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/ggikahcrr.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gwmtncekm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gmbclinox.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gzjmrluyp.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gmiwpqyit.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ghhqgqmiy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/geoohtkvb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gumkgzqil.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gnrgbbhbl.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gxdcnrhkm.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/ghcpcqgix.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gsozllpht.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ghiauhkth.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gpuwwsmmw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gfkyvztgk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/glmarnnxg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gpvasnoum.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gpryydoko.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gtpltyknd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gogpujgaj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gqgftzmrv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gyuezkekv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gfjanoqxb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/glexejhdh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/ggtuxukvb.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gitbdnabb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gifnmnygd.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/glktzftaj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gpqmqizac.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/geyccpacn.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gewzjobwf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gjytauqtr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gvwkqzjxb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gbyjktsli.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/glioztfcz.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/giqqotels.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqlmeduxr.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gjmzqpoha.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtctisrzg.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gepxeucbc.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/guyvazxyg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gqhysywnq.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gonoqxbhe.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gnqcwayuk.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/ghfucerpc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvqlmqwxn.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gtsvhvwql.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gewomvyyt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/glihbjtzc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gprlktdia.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gslvgypxg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gjrurhffz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gfqygplpc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gggjhlmkd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gfyaeppfi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gbnauvjwp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gtolszvpo.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gdihyhfex.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gifrctbnd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gflftflxq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gjhrqcwyk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gmpnxvfwx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gpmmdidua.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/ghnvhapjo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/glqgglasi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gmnnbnosg.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gnlezyvky.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmdnedbdp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gdiiuwdrr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gqnojyzxu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gbbprhqrh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gakhnjweo.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gewwdxuzq.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gmhmoeoco.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gvvstuawh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/ggnnmefaf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/ggwzukmow.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gbsimbeio.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/guaacgeej.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gfwzfeixl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gjtdbcver.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/giwotzsey.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gxgsvteel.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gvvrxghoa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gohkrtxoy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gcrdyexib.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gsvfmywxp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gzkpghwns.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gqoihubba.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gnzbnlqvg.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gqkvhafiz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gbnkmlpft.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gkhgpumop.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gxrjyfltc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gnulstusg.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gzhafrhxf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gdvqekjjf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gnvawbjke.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gcemxalfu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gjybejyfc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gldkrtvir.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gxxexbsey.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gwifshhhv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gdngzctlv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gakhoqolg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gqhemzetl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gzvujhqfj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gcwbmxetm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gmsdmsuln.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gqmzjpcmk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gaahxanvq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gftrlliur.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gpuberhrx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gecnehqjw.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gvrpolkqo.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gpiyrtmpu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gazjamnow.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gsoxmhmxq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gtoutpuwh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gutnhtyza.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gitfpivds.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gurzrzxcg.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/ghuctkokb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gxpiwznjt.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gdehwiorb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gbffqyaiq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gcdcvgjur.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gcgakmhpw.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/grphvialk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/guxbudomz.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ghrbgykkg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/glocwgfwb.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gunwmplym.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gzfdihrac.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gxkdcmhvf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gnefkdgnc.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gpedzfhod.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gfnsasxjr.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/giayprzhf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/glmdakyik.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/grwdycejl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gezrghaby.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gdqesdezw.sHtML


<!-- 参考信息 -->