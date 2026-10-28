代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtsneznipz.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtfuugaqfe.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtfvzdrwko.html

[R55] 压缩与解压
来源：http://hz.zycfv.cn/gtxvzxgpgp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgufenzy.top/gtgzhkfhev.html

[R56] 远程拷贝
来源：http://hz.yonumen.top/gtckpzoiqk.html

scp file user@host:/path/
来源：http://hz.jinghuilouyu.cn/gthwtzkspv.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtmrfoleus.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtnabcvqqh.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtflninzkq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangshuangyany.cn/gtlhcsmxui.html

[R59] 发 POST JSON
来源：http://hz.gogol.net.cn/gtjshbtvdn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuetiantiany.cn/gtwelhrjcz.html

[R60] 只看 HTTP 状态码
来源：http://hz.gaohongyu789.top/gteucuzxsv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtidyhredw.html

[R61] 磁盘占用
来源：http://hz.ppjwa.cn/gtcdmvhcuu.html

df -h;  du -sh *
来源：http://hz.gogol.net.cn/gtmgppoeqc.html

[R62] 找最占空间的文件
来源：http://hz.zhiwuduotai.top/gteixipgbq.html

du -ah . | sort -rh | head -10
来源：http://hz.xziqi.cn/gtgcibtbdh.html

[R63] 内存与进程
来源：http://hz.kuanghao11.cn/gtcvohpush.html

free -h;  ps aux | grep nginx
来源：http://hz.tianlin.xyz/gtongopbmy.html

[R64] 结束进程
来源：http://hz.gotoacloud.top/gthdlfuvij.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtvwidrmyv.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gtbkhowsos.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.0kj1m.cn/gtnosbgtbl.html

[R66] 定时任务
来源：http://hz.yj202588.top/gtnuynklpm.html

crontab -e;  crontab -l
来源：http://hz.zhixingplan.top/gtdnmtzoaf.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gtnerbhxug.html

openssl rand -hex 16
来源：http://hz.hysaishi.cn/gtfyydgtoe.html

[R68] 计算文件校验值
来源：http://hz.fzhhl.top/gtubtpstgi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gtgoijintn.html

[R69] 生成随机密码
来源：http://hz.zhaomingkeji.xyz/gtpiuihcdq.html

head -c 16 /dev/urandom | base64
来源：http://hz.cqqwz.cn/gtfepnypig.html

[R70] 时间戳与互转
来源：http://hz.gogol.net.cn/gtlkduaoxv.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtounitzsl.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtwxjqnqhr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yanxiufei.cn/gtpoeqjbtk.html

[R72] 等待端口就绪
来源：http://hz.hammf.cn/gtbvlflebp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ivvv.top/gtzzyhopbb.html

[R73] 分割大日志
来源：http://hz.xuanzx.com/gtmbmmrlge.html

split -l 1000 big.log part_
来源：http://hz.cashguo.top/gtrqdwjbrc.html

[R74] 批量重命名
来源：http://hz.0kj1m.cn/gtljmgcnja.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sysykeji.top/gtliypowmk.html

[R75] 导出环境变量
来源：http://hz.birdmap.top/gtucihkfdf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xingfuxueyuan.xyz/gtknjjeluc.html

[R76] 使用临时文件
来源：http://hz.wangdashe.top/gtyrwxcagb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtmzfkryyx.html

[R77] 读取用户输入
来源：http://hz.yongpay.top/gtopijuxzf.html

read -rp "请输入: " ans
来源：http://hz.ppjwa.cn/gtlzarcbrs.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtugjsetfu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aibaodan.cn/gtmqcpkmpq.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtaejjklay.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gthnxqpreg.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtnxwvlcez.html

time ./run.sh
来源：http://hz.hongshengwenyu.top/gtvqgqahud.html

================================================================================
来源：http://hz.sufxvd.cn/gtdrwxliuc.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtsvazawlu.html

================================================================================
来源：http://hz.havefunace.top/gtlzwlhqvs.html

[S01] C：Hello World
来源：http://hz.jiagoushi.top/gtevzqgell.html

#include <stdio.h>
来源：http://hz.xinyue.icu/gtzysxlvym.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.smart0.xyz/gtqhfpcabf.html

[S02] C：变量与格式化输出
来源：http://hz.feifeiyinyue.top/gtkuoljnqx.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gtqljbdimi.html

[S03] C：读入整数
来源：http://hz.ivvv.top/gtvvcuaevl.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtzduzgpns.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtmjmnrbjp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigfzy.top/gtnadtxjsm.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtwztzmfjl.html

strlen(s)
来源：http://hz.cdnleiting.top/gtaeuxdaqp.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtmtcqfikh.html

strcmp(a, b) == 0
来源：http://hz.jinyuanbaomall.cn/gtqwuevqlc.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gtghnglegp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gaohongyu789.top/gtxvwfplnu.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtcgkaqauy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtcrsikkqo.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtnlwvkgmq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gtubfbmmvp.html

[S10] C：指针与解引用
来源：http://hz.xuetiantiany.cn/gtjdprvslv.html

int *p = &a;  *p = 5;
来源：http://hz.jinghuilouyu.cn/gttyjzyfqy.html

[S11] C：逐行读文件
来源：http://hz.yonumen.top/gtrfsjpouc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gaohongyu789.top/gtngsmgrml.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtlwfridni.html

fclose(f);
来源：http://hz.9152youxi.cn/gtvskbibnk.html

[S12] C：写文件
来源：http://hz.sufxvd.cn/gtglimycze.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhijiandao.cn/gtoeiebdio.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtrthvlnth.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.meibo888.top/gtxiqxnxez.html

[S14] C：枚举
来源：http://hz.zhoulong.xyz/gtsdomndxg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydzc1.top/gtelwxaewo.html

[S15] C：类型转换
来源：http://hz.bjfxy.top/gtkgassvlb.html

(double) a / b
来源：http://hz.cqqwz.cn/gtqdrcaaor.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gttgifcfap.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtfctugtcw.html

[S17] C：安全拼接字符串
来源：http://hz.jinghuilouyu.cn/gtccnyuutc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigufen.top/gtjzgfzbjm.html

[S18] C：命令行参数
来源：http://hz.kuanghao11.cn/gtexdpzqfi.html

int main(int argc, char **argv)
来源：http://hz.bjfxy.top/gtcjdygcbn.html

[S19] C：快速排序
来源：http://hz.wangshuangyany.cn/gthzvxreto.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtiehhndmy.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gtaeshggaa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtaohpeypi.html

[S21] C：字符类别判断
来源：http://hz.sxryk.cn/gtkcrwepjm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtdmrjpwbz.html

[S22] C：字符串转数字
来源：http://hz.gzhubu.top/gtqkebzhhn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gterdibcal.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gthqxfhviu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.meibo888.top/gtyqduhkmb.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtrjnraupe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangshuangyany.cn/gtfiptbsgl.html

[S25] C：内存拷贝
来源：http://hz.yuxming.cn/gtwjigfgok.html

memcpy(dst, src, n);
来源：http://hz.sufxvd.cn/gtlwxvccpj.html

[S26] C：内存清零
来源：http://hz.daria6918.cn/gtrwkbajdq.html

memset(a, 0, sizeof a);
来源：http://hz.guannengcc.top/gtjkmeqmbr.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtvnloehug.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtfksdiylo.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtnjjwahqr.html

static int counter = 0;
来源：http://hz.feifeiyinyue.top/gtqikopqem.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtrzimrdfm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtemjjcgsz.html

[S30] C：头文件保护
来源：http://hz.quarkkingdee.top/gtfftxicyk.html

#ifndef X_H
来源：http://hz.havefunace.top/gtfzktkopl.html

#define X_H
来源：http://hz.zycfv.cn/gtwmorxspf.html

#endif
来源：http://hz.yj202588.top/gtaqmqgtzr.html

[S31] C++：Hello World
来源：http://hz.nanxuanxn.top/gtagpcrogv.html

#include <iostream>
来源：http://hz.9152youxi.cn/gtmogxycgw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnxiangtu.top/gtblaoimdb.html

[S32] C++：字符串
来源：http://hz.hongshengwenyu.top/gteyqtfjca.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtvxwrjsxo.html

[S33] C++：vector 增删
来源：http://hz.zhiwuduotai.top/gtnkneoqev.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtxxmnrtds.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gtlukktyqc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtakxciswy.html

[S35] C++：map
来源：http://hz.guowangkeji.top/gtnsmvyusg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtsrgytqzb.html

[S36] C++：unordered_map
来源：http://hz.yj202588.top/gtqgqkyngc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtbfkpsavo.html

[S37] C++：set
来源：http://hz.52xcode.cn/gtyhncsupw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtkwrcuaih.html

[S38] C++：排序
来源：http://hz.xingfuxueyuan.xyz/gttlfytrse.html

std::sort(v.begin(), v.end());
来源：http://hz.hysaishi.cn/gtmhubeoyp.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtsyxsufws.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gtjproqqbx.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtwdslgdtv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtcpdeuhjj.html

[S41] C++：类与构造函数
来源：http://hz.hfpthk.cn/gtmudlbqhy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.smart0.xyz/gtzxnckuvo.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtcjvfdmuq.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtlktrugub.html

[S43] C++：智能指针
来源：http://hz.yj20258888.top/gtlebifgvb.html

auto p = std::make_unique<int>(5);
来源：http://hz.jlsjyb.cn/gtetkftrvs.html

[S44] C++：引用传参
来源：http://hz.shzxlz.cn/gtekecumiv.html

void inc(int &x) { ++x; }
来源：http://hz.gzhubu.top/gtemqdgxdd.html

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtexrxdxqr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jyoumei.cn/gtfvrkjlxj.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gtimoeiwsf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtjmpyhlmp.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgufenzy.top/gtycudbpjt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtenanrnvl.html

[S48] C++：逐行读文件
来源：http://hz.svipenyu.cn/gtpfmzmrwk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinyuanbaomall.cn/gtnwvnmjhr.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gttsjpvika.html

[S49] C++：写文件
来源：http://hz.cqqwz.cn/gtrynywfrb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.316326.xyz/gtzkjmssim.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtecrzgtyf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gttiijeqol.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gttqugrpcz.html

static_cast<double>(a) / b
来源：http://hz.chenlongwang.top/gtzagjyfra.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtjrgfiqiu.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gtcgntcicv.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtnjdpdkog.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtghmkoclr.html

[S54] C++：异常处理
来源：http://hz.0kj1m.cn/gtmaegdeld.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gtnfkbecqh.html

[S55] C++：结构化绑定
来源：http://hz.jiagoushi.top/gtgxmydlcx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuetiantiany.cn/gtefvonbjv.html

[S56] C++：optional
来源：http://hz.tian-w.cn/gtbuvymukc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.c1oappe.top/gtkvvguqxq.html

[S57] C++：编译期常量
来源：http://hz.daria6918.cn/gtzodlrlxa.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gtohkqsrwc.html

[S58] C++：命名空间
来源：http://hz.ybcxt.top/gtucbjzyvc.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtxreioyzh.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtymxlydyh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangshuangyany.cn/gtyzwhxabq.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtuxyhcanc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ehwqpu.com/gtkidbntsi.html

================================================================================
来源：http://hz.andypj.xyz/gtitvaftdu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtqlfeoamo.html

================================================================================
来源：http://hz.cqqwz.cn/gtiiqhrljx.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gtmzbkmtnz.html

println("Hello")
来源：http://hz.yueranfly.top/gtowyejblk.html

[T02] Kotlin：变量
来源：http://hz.hongshengwenyu.top/gtwqczdfta.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtsekybbgq.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gtdxcmwlno.html

"值: $b"
来源：http://hz.kuanghao11.cn/gthkhqgmzi.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtuctmmqor.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtfqzywpht.html

[T05] Kotlin：when 表达式
来源：http://hz.hfpthk.cn/gtdnjjbyms.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj202588.top/gtnbpcoxoa.html

[T06] Kotlin：集合映射
来源：http://hz.aizwys.cn/gtpettxwor.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuetiantiany.cn/gtyjorbyxt.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gtmnnbtsey.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gthiotzxzk.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtqfyrpjcw.html

data class User(val name: String, val age: Int)
来源：http://hz.quarkkingdee.top/gtgrjctvpr.html

[T09] Kotlin：扩展函数
来源：http://hz.zhoulong.xyz/gtshvfzkok.html

fun String.exclaim() = this + "!"
来源：http://hz.shzxlz.cn/gtjoyqycgd.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gtybtnyhzh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydjk.org.cn/gttpurkrhx.html

[T11] Kotlin：协程
来源：http://hz.yj20258.top/gtbehrukjw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zdqjudy.top/gtkywxousj.html

[T12] Kotlin：解构声明
来源：http://hz.tianlin.xyz/gtftrqikea.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258888.top/gtmiwphszr.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxinkj.top/gtzkfjhnhx.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gttwaaqmms.html

[T14] Kotlin：循环
来源：http://hz.jqgfzy.top/gtemvhlsyx.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtpgdxzlfr.html

[T15] Kotlin：接口
来源：http://hz.zhijiandao.cn/gtunpaxkjl.html

interface Shape { fun area(): Double }
来源：http://hz.havefunace.top/gtzuozkwgs.html

[T16] Swift：Hello World
来源：http://hz.yongpay.top/gtpaicjazx.html

print("Hello")
来源：http://hz.zdqjudy.top/gtzjghthhl.html

[T17] Swift：变量与常量
来源：http://hz.shangyingyoupin.top/gtnvmhgrdd.html

var a = 1;  let b = 2
来源：http://hz.guannengcc.top/gttcjwrxax.html

[T18] Swift：字符串插值
来源：http://hz.fengsongda.top/gtyyobxadi.html

"值: \(b)"
来源：http://hz.xylfe.cn/gthztlirks.html

[T19] Swift：可选绑定
来源：http://hz.ydzc1.top/gtbcwnccft.html

if let n = opt { print(n) }
来源：http://hz.hnxiangtu.top/gtdngfrrmj.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gtzwoaskux.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuetiantiany.cn/gtycsadlmv.html

[T21] Swift：遍历
来源：http://hz.cashguo.top/gtffxfmels.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtsvqqjrdd.html

[T22] Swift：字典
来源：http://hz.hysaishi.cn/gtuokrpjai.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.meibo888.top/gtpvprytti.html

[T23] Swift：函数
来源：http://hz.52xcode.cn/gtfugaciah.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gtqicubqfo.html

[T24] Swift：闭包
来源：http://hz.xuanzx.com/gtlbvyqgkc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yongpay.top/gttuydkjua.html

[T25] Swift：结构体
来源：http://hz.gotoacloud.top/gtpnyebzph.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtupikuzpi.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtxxofyrdj.html

class A: Base { override func f() {} }
来源：http://hz.hammf.cn/gtihrirxiy.html

[T27] Swift：错误处理
来源：http://hz.c1oappe.top/gtanwenvjv.html

do { try f() } catch { print(error) }
来源：http://hz.cashguo.top/gtplkttute.html

[T28] Swift：枚举
来源：http://hz.birdmap.top/gttryesrdq.html

enum Color { case red, green }
来源：http://hz.nwbrower.top/gtrhjzqcpr.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtnngzgztv.html

guard let x = opt else { return }
来源：http://hz.bjfxy.top/gtadedevma.html

[T30] Swift：协议
来源：http://hz.gogol.net.cn/gtcdejlbqp.html

protocol Shape { func area() -> Double }
来源：http://hz.cucudq.cn/gtvsgdlbuc.html

[T31] Lua：Hello World
来源：http://hz.hongshengwenyu.top/gtstqfkufm.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtxfzckkbg.html

[T32] Lua：局部变量
来源：http://hz.pengpengdd.cyou/gtcfzbeuaw.html

local a = 1
来源：http://hz.yvedp.cn/gtnhhzzsui.html

[T33] Lua：表（数组）
来源：http://hz.shuidangran.top/gtoyezicta.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ehwqpu.com/gtpxkciapq.html

[T34] Lua：遍历表
来源：http://hz.ydjk.org.cn/gtzkwdzohw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenlongwang.top/gtabupmbrn.html

[T35] Lua：字典表
来源：http://hz.dianchejie.cn/gtvjcqcpmf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhongyouzk.top/gtxnqskkrp.html

[T36] Lua：函数
来源：http://hz.pycfn.com/gthdalxena.html

function add(a, b) return a + b end
来源：http://hz.birdmap.top/gtmnxzmwuw.html

[T37] Lua：字符串拼接
来源：http://hz.xylfe.cn/gtrowhlzez.html

"a" .. "b"
来源：http://hz.jiagoushi.top/gtqqmibeli.html

[T38] Lua：条件
来源：http://hz.aizwys.cn/gtobeipbew.html

if x > 0 then print("正") end
来源：http://hz.shzxlz.cn/gtzcnwrwdt.html

[T39] Lua：模式匹配
来源：http://hz.vqdsnc.cn/gthzqzjtde.html

string.find(s, "%d+")
来源：http://hz.yonumen.top/gtvoudzfgg.html

[T40] Lua：元表
来源：http://hz.hywenlv.cn/gttgftqxkc.html

setmetatable({}, { __index = base })
来源：http://hz.daxiang520.top/gtwdtkehuf.html

[T41] Perl：Hello World
来源：http://hz.cheryme.top/gtvrhvdvvv.html

print "Hello\n";
来源：http://hz.aizwys.cn/gtubnvhyjs.html

[T42] Perl：变量类型
来源：http://hz.gogol.net.cn/gthpiuaoja.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.52xcode.cn/gtvscpuhse.html

[T43] Perl：字符串插值
来源：http://hz.nwbrower.top/gtubiieudp.html

"值: $a"
来源：http://hz.snrcjt.cn/gtmwjmsbnl.html

[T44] Perl：条件
来源：http://hz.zhixingplan.top/gtxgrsfeql.html

if ($a > 0) { print "正"; }
来源：http://hz.ppjwa.cn/gtvnqlkeim.html

[T45] Perl：数组遍历
来源：http://hz.daxiang520.top/gtyrhbnwlr.html

for my $x (@arr) { print $x; }
来源：http://hz.wangdashe.top/gtjfjnervu.html

[T46] Perl：哈希操作
来源：http://hz.gzhubu.top/gtcklflsgt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgfzy.top/gtlbpfgcos.html

[T47] Perl：正则捕获
来源：http://hz.9152youxi.cn/gttdqctnbi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sysykeji.top/gtmmumnjhq.html

[T48] Perl：正则替换
来源：http://hz.ivvv.top/gtxahcgbwq.html

$s =~ s/old/new/g;
来源：http://hz.chenjidiqi.icu/gtizswzwme.html

[T49] Perl：函数
来源：http://hz.ywan-chungtsiang.top/gtqpragdmq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yvedp.cn/gtluotxjfw.html

[T50] Perl：逐行读文件
来源：http://hz.shuidangran.top/gtgmpcbicw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinyuanbaomall.cn/gtejmtttfa.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.meibo888.top/gtvqikxthv.html

[T51] Scala：Hello World
来源：http://hz.ybcxt.top/gtmbcuhnit.html

println("Hello")
来源：http://hz.hywenlv.cn/gtyasybdjx.html

[T52] Scala：变量
来源：http://hz.yj202588.top/gtczneyntm.html

val a = 1;  var b = 2
来源：http://hz.andypj.xyz/gtorygffyn.html

[T53] Scala：字符串插值
来源：http://hz.snrcjt.cn/gtfbjfbycr.html

s"值: $b"
来源：http://hz.9152youxi.cn/gteebwvkmb.html

[T54] Scala：集合映射
来源：http://hz.yueranfly.top/gtnjqpmocp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxuanxn.top/gtffhogwdx.html

[T55] Scala：集合过滤
来源：http://hz.shangyingyoupin.top/gtdetppqoq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhiwuduotai.top/gtoabvprdp.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gtpltlowpm.html


<!-- 参考信息 -->