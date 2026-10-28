代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtbztipdik.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtjyaikfqs.html

wc -l a.txt
来源：http://hz.yj202588.top/gtsnddihyz.html

[R53] 查看文件头与实时尾
来源：http://hz.chenjidiqi.icu/gtphyzanff.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtqgyporae.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtrcyyrxuc.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtiopoyeea.html

[R55] 压缩与解压
来源：http://hz.bjfxy.top/gtbbvgxqrr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgufenzy.top/gtxjeiydxi.html

[R56] 远程拷贝
来源：http://hz.bjfxy.top/gtexaduelb.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtpchggkax.html

[R57] 远程执行命令
来源：http://hz.xziqi.cn/gtukrqujwe.html

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtgyqhxgtk.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtjygoyzsl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtrcrtmztn.html

[R59] 发 POST JSON
来源：http://hz.yvedp.cn/gthbbzoexz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtbpbwscks.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258.top/gtbwbwwsuq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dianchejie.cn/gtlicnbezl.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtfesfdzom.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtmjqjudik.html

[R62] 找最占空间的文件
来源：http://hz.jinqigfzy.top/gtuozgnxip.html

du -ah . | sort -rh | head -10
来源：http://hz.0kj1m.cn/gtvsjmidqf.html

[R63] 内存与进程
来源：http://hz.0kj1m.cn/gtkfmhvpho.html

free -h;  ps aux | grep nginx
来源：http://hz.xuetiantiany.cn/gtbvhrovxf.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gthqhaorjt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtyzggxpwm.html

[R65] 查看端口占用
来源：http://hz.zycfv.cn/gtqgsedjug.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtnshymjgs.html

[R66] 定时任务
来源：http://hz.cqqwz.cn/gtakrkfirw.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gtlormqbah.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gtuivwkunz.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtzilibsgg.html

[R68] 计算文件校验值
来源：http://hz.fengsongda.top/gtpejwmufx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhiwuduotai.top/gtaeadmaaw.html

[R69] 生成随机密码
来源：http://hz.xuanzx.com/gtavaiwokk.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtgbvfjewv.html

[R70] 时间戳与互转
来源：http://hz.dashuyun.cn/gtfjlxsmbl.html

date +%s;  date -d @1700000000
来源：http://hz.yj202588.top/gtvdrwkvqb.html

[R71] 日期格式化
来源：http://hz.sufxvd.cn/gtqhfsybka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hysaishi.cn/gtawhehlll.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtapufqilf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtpnrlvnpz.html

[R73] 分割大日志
来源：http://hz.sxryk.cn/gtcpisbqhq.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtrjxsielm.html

[R74] 批量重命名
来源：http://hz.pengpengdd.cyou/gtdmckivhf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtjigamhoy.html

[R75] 导出环境变量
来源：http://hz.hfpthk.cn/gtrzrannit.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sweek.top/gtdnutgbnd.html

[R76] 使用临时文件
来源：http://hz.52xcode.cn/gtnsbqwzvh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtvstptqej.html

[R77] 读取用户输入
来源：http://hz.aizwys.cn/gtdfhwybpk.html

read -rp "请输入: " ans
来源：http://hz.feifeiyinyue.top/gtghjalzaq.html

[R78] 交互式菜单
来源：http://hz.redwolf501.top/gtgbvlzano.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jyoumei.cn/gtneylhzme.html

[R79] 解析命令行选项
来源：http://hz.sweek.top/gtpiucidih.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtkwqkoiwg.html

[R80] 查看脚本执行耗时
来源：http://hz.gogol.net.cn/gtirdbihva.html

time ./run.sh
来源：http://hz.xinyue.icu/gtdkgsrffl.html

================================================================================
来源：http://hz.haohaochexian.top/gtrzurcyuq.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtbbsxlnzn.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjlinzgyb.html

[S01] C：Hello World
来源：http://hz.birdmap.top/gtsrrxunvg.html

#include <stdio.h>
来源：http://hz.ehwqpu.com/gtudoeoxut.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.9152youxi.cn/gtoizminvn.html

[S02] C：变量与格式化输出
来源：http://hz.tanke756.top/gtqkdnxlhz.html

int a = 10; printf("%d\n", a);
来源：http://hz.vqdsnc.cn/gterxoypxu.html

[S03] C：读入整数
来源：http://hz.dianchejie.cn/gtchubknyu.html

int x; scanf("%d", &x);
来源：http://hz.dianchejie.cn/gtstliwqpb.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtvetuxson.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hfpthk.cn/gtxoomlvmb.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gttzalqudq.html

strlen(s)
来源：http://hz.yonumen.top/gtlwqznlhh.html

[S06] C：字符串比较
来源：http://hz.ydzc1.top/gtnrdjflfn.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtbjivhzbv.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtvmtxagoi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.snrcjt.cn/gtxolhflra.html

[S08] C：动态内存分配与释放
来源：http://hz.zhengqikj.top/gthlgdylxn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.bjfxy.top/gtgcobwush.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gthdamlkyg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtvvjhbddf.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtuasdjfsx.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gtwwjmaugy.html

[S11] C：逐行读文件
来源：http://hz.ydzc1.top/gtpielvrgc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sufxvd.cn/gtsyhzkoyt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuanzhike.top/gthurefrej.html

fclose(f);
来源：http://hz.haohaochexian.top/gtaaioqfrj.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gtdryopjmo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.bjfxy.top/gtwlbjrvki.html

[S13] C：宏定义
来源：http://hz.tianlin.xyz/gtwiimtnod.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinyuanbaomall.cn/gtmbmvemjj.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtfrinsczd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hysaishi.cn/gtdldxagre.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtclfdoufb.html

(double) a / b
来源：http://hz.chenzaomai.com/gtakfxrmhr.html

[S16] C：位操作置位
来源：http://hz.kuanghao11.cn/gtllfvgesm.html

x |= (1 << 3);
来源：http://hz.jinyuanbaomall.cn/gtrdjgwjfg.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gtynrzhmpi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gttsnqzzxa.html

[S18] C：命令行参数
来源：http://hz.cashguo.top/gtocgrqvlf.html

int main(int argc, char **argv)
来源：http://hz.bjfxy.top/gtuxaibhvj.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gttcmndcuh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtwpznrvzc.html

[S20] C：二分查找
来源：http://hz.yongpay.top/gtnuwfrccg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtjkmkbuqf.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtfcjgvrmb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gthaynoqbb.html

[S22] C：字符串转数字
来源：http://hz.cdnleiting.top/gtyskrostg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhixingplan.top/gtuugnwtya.html

[S23] C：随机数
来源：http://hz.cashguo.top/gtetzwljyv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtnwcpgygh.html

[S24] C：获取本地时间
来源：http://hz.nanxinkj.top/gtmbvpyaff.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenjidiqi.icu/gtqqtgnsth.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gtwrkxprkx.html

memcpy(dst, src, n);
来源：http://hz.nwbrower.top/gtnteprcfe.html

[S26] C：内存清零
来源：http://hz.yuanzhike.top/gtanrcnfvp.html

memset(a, 0, sizeof a);
来源：http://hz.zhijiandao.cn/gtispbjzir.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtahtbgjvi.html

const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtdiclmifx.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtzjwgkgzu.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtobjyuamu.html

[S29] C：变参函数
来源：http://hz.jinyuanbaomall.cn/gtcmzbmicf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.9152youxi.cn/gtaffwvtld.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtrrthymlf.html

#ifndef X_H
来源：http://hz.dashuyun.cn/gthcszxhfi.html

#define X_H
来源：http://hz.316326.xyz/gtynmbaogw.html

#endif
来源：http://hz.shanyushiyangkeji.top/gtwwncqjzp.html

[S31] C++：Hello World
来源：http://hz.birdmap.top/gtclgdrsfw.html

#include <iostream>
来源：http://hz.xuetiantiany.cn/gtawollfwi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtbyoibdyf.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gttvfcpjon.html

std::string s = "hi";  s += "!";
来源：http://hz.yonumen.top/gtsfpsuojd.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtnxidhnqt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtroqiycvo.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtzcwrnesl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.mhx1999.top/gtygxfbsxb.html

[S35] C++：map
来源：http://hz.svipenyu.cn/gtljppbymq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gtkebrgtzu.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtvqqldyhp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtnnratfoi.html

[S37] C++：set
来源：http://hz.sweek.top/gtpacditnp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtdmhmiplt.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtadbjrnto.html

std::sort(v.begin(), v.end());
来源：http://hz.mhx1999.top/gtiaussrmh.html

[S39] C++：自定义比较器排序
来源：http://hz.zhijiandao.cn/gtzvwhvqus.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tian-w.cn/gtebpknfeb.html

[S40] C++：查找元素
来源：http://hz.shuidangran.top/gtpdbiogrg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj202588.top/gtanvwdsbu.html

[S41] C++：类与构造函数
来源：http://hz.fzhhl.top/gtycpxssga.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtfjegcblr.html

[S42] C++：继承与虚函数
来源：http://hz.sufxvd.cn/gtyuncevis.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gtkipmelfs.html

[S43] C++：智能指针
来源：http://hz.sxryk.cn/gtibazmpqy.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuanzhike.top/gtnclkpeme.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gtyiwnqxzn.html

void inc(int &x) { ++x; }
来源：http://hz.zdqjudy.top/gthmtebvoe.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gtdjsbiohp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuanzx.com/gtjgqxkbcp.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtsmfhlwcs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dianchejie.cn/gtjxprdxyj.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj202588.top/gtbvmqtrnf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daxiang520.top/gtivuyhbps.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtsodnvpaa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cucudq.cn/gtijbverdb.html

while (std::getline(in, line)) { }
来源：http://hz.aibaodan.cn/gtzqojbpuf.html

[S49] C++：写文件
来源：http://hz.ydjk.org.cn/gtqvpkhnpx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtrxaiyxkz.html

[S50] C++：格式化数字
来源：http://hz.yanxiufei.cn/gtvetcauaf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gteodnwjwk.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtcewiaaly.html

static_cast<double>(a) / b
来源：http://hz.ybcxt.top/gtfvbahapo.html

[S52] C++：const 与 noexcept
来源：http://hz.dianchejie.cn/gtjsacttnn.html

int size() const noexcept { return n_; }
来源：http://hz.cashguo.top/gtkzvcwiqd.html

[S53] C++：移动语义
来源：http://hz.xuetiantiany.cn/gtjnjtuchx.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtifhewzky.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtjvuwywqs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hywenlv.cn/gtsjyfskuc.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gtkhetvkmc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuetiantiany.cn/gtsrzpqmlg.html

[S56] C++：optional
来源：http://hz.birdmap.top/gtfqrysbnq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtygdlnpkp.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangtech.top/gtdkvkrlaq.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtanwtilvd.html

[S58] C++：命名空间
来源：http://hz.dashuyun.cn/gtbvmnjhbf.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuanzx.com/gtrszwizob.html

[S59] C++：静态断言
来源：http://hz.cashguo.top/gttvymylms.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnqzz.top/gtnhdxjasv.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtcdygjkwt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtmjhgrhky.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpziwkyvn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtoqpkxaqh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvlkwaemg.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtzadudueo.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtgcbewujh.html

[T02] Kotlin：变量
来源：http://hz.yuanzhike.top/gtxrwvqwvn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtryxadiry.html

[T03] Kotlin：字符串模板
来源：http://hz.hywenlv.cn/gtxnhytsci.html

"值: $b"
来源：http://hz.guannengcc.top/gtlaariugn.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtutsfkirz.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gteuigxops.html

[T05] Kotlin：when 表达式
来源：http://hz.guowangkeji.top/gtlafugtvk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sweek.top/gtewoekihx.html

[T06] Kotlin：集合映射
来源：http://hz.zdqjudy.top/gtedtijldv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cheryme.top/gtinagozzs.html

[T07] Kotlin：集合过滤
来源：http://hz.xuanzx.com/gtpieklqzi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangdashe.top/gtoayimoyw.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtjygcjqdu.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtrnhovtfp.html

[T09] Kotlin：扩展函数
来源：http://hz.ehwqpu.com/gtfdczelkt.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtuityuxkb.html

[T10] Kotlin：默认参数
来源：http://hz.smart0.xyz/gtwegisdae.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fengsongda.top/gtvgbcfasw.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gtbpcaivqw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hywenlv.cn/gtwvtifqat.html

[T12] Kotlin：解构声明
来源：http://hz.cqqwz.cn/gteqqygsyc.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj202588.top/gtvtylvfyd.html

[T13] Kotlin：只读 Map
来源：http://hz.yangfankeji.com/gtgyzkkhlc.html

val m = mapOf("a" to 1)
来源：http://hz.chenlongwang.top/gtdemazhdw.html

[T14] Kotlin：循环
来源：http://hz.wangdashe.top/gtrabguzsw.html

for (i in 1..10) println(i)
来源：http://hz.tianlin.xyz/gtfnqxyjwb.html

[T15] Kotlin：接口
来源：http://hz.cheryme.top/gtiivqhxui.html

interface Shape { fun area(): Double }
来源：http://hz.yuxming.cn/gtilzaoaxf.html

[T16] Swift：Hello World
来源：http://hz.zhixingplan.top/gtgbqzgcpd.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtbrdrmaez.html

[T17] Swift：变量与常量
来源：http://hz.jinyuanbaomall.cn/gtpaexztho.html

var a = 1;  let b = 2
来源：http://hz.xingfuxueyuan.xyz/gtxcjgcrbt.html

[T18] Swift：字符串插值
来源：http://hz.gotoacloud.top/gtlzgabvmp.html

"值: \(b)"
来源：http://hz.hammf.cn/gtqdwkcjdq.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gtexljpixm.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtmcokgwkr.html

[T20] Swift：数组操作
来源：http://hz.cashguo.top/gtkbawfgxc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gtgamxetpv.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gtpjyjegbq.html

for x in a { print(x) }
来源：http://hz.fengsongda.top/gticvpbbha.html

[T22] Swift：字典
来源：http://hz.jinghuilouyu.cn/gtfgprvjum.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jlsjyb.cn/gtlygqhfih.html

[T23] Swift：函数
来源：http://hz.haohaochexian.top/gtpcbgtyex.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gtdwvjovlu.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gtdejdrkwr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.bjfxy.top/gtkxykoovi.html

[T25] Swift：结构体
来源：http://hz.sweek.top/gtuzrqfrwp.html

struct P { var x: Int }
来源：http://hz.dianchejie.cn/gtwmhuhcgu.html

[T26] Swift：类与重写
来源：http://hz.aibaodan.cn/gtwvxroaqz.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtvvynysab.html

[T27] Swift：错误处理
来源：http://hz.fengsongda.top/gttpcpiisp.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gtmqujskwm.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangkeji.top/gtaalrfeof.html

enum Color { case red, green }
来源：http://hz.xylfe.cn/gtwaaoeqyj.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtjtavwodn.html

guard let x = opt else { return }
来源：http://hz.cqqwz.cn/gtojnipema.html

[T30] Swift：协议
来源：http://hz.sxryk.cn/gtjgtmwuem.html

protocol Shape { func area() -> Double }
来源：http://hz.yanxiufei.cn/gtnwapwmxb.html

[T31] Lua：Hello World
来源：http://hz.zhengqikj.top/gtiatenisc.html

print("Hello")
来源：http://hz.andypj.xyz/gtpkmivsmy.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtgjsvwwdq.html

local a = 1
来源：http://hz.zhaomingkeji.xyz/gtfgapnkfh.html

[T33] Lua：表（数组）
来源：http://hz.ydjk.org.cn/gtpngdgpty.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtdugorjbb.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtrpusziij.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.feifeiyinyue.top/gtbcfrbcwi.html

[T35] Lua：字典表
来源：http://hz.jinqigufen.top/gtvzboevif.html

local d = { a = 1 };  d.b = 2
来源：http://hz.haohaochexian.top/gtfhtmwifq.html

[T36] Lua：函数
来源：http://hz.sxryk.cn/gtxlusewuk.html

function add(a, b) return a + b end
来源：http://hz.shuidangran.top/gtfdntwovq.html

[T37] Lua：字符串拼接
来源：http://hz.tianlin.xyz/gtvdhudwdq.html

"a" .. "b"
来源：http://hz.52xcode.cn/gtwzubdmfs.html

[T38] Lua：条件
来源：http://hz.xinyue.icu/gthrtfazkh.html

if x > 0 then print("正") end
来源：http://hz.feifeiyinyue.top/gtjdjcwvpr.html

[T39] Lua：模式匹配
来源：http://hz.xziqi.cn/gtiugiirrt.html

string.find(s, "%d+")
来源：http://hz.yanxiufei.cn/gtxizcbtva.html

[T40] Lua：元表
来源：http://hz.hnxiangtu.top/gtbfmuxplt.html

setmetatable({}, { __index = base })
来源：http://hz.snrcjt.cn/gtgcaqmecg.html

[T41] Perl：Hello World
来源：http://hz.kuanghao11.cn/gtqpmdsirl.html

print "Hello\n";
来源：http://hz.svipenyu.cn/gtjtmlhtew.html

[T42] Perl：变量类型
来源：http://hz.shanyushiyangkeji.top/gtiyasxhwp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhiwuduotai.top/gtwjgunnff.html

[T43] Perl：字符串插值
来源：http://hz.jlsjyb.cn/gtvjfmkzsx.html

"值: $a"
来源：http://hz.iojbl.cn/gtqekpvdcj.html

[T44] Perl：条件
来源：http://hz.yj20258.top/gtrvftorib.html

if ($a > 0) { print "正"; }
来源：http://hz.yvedp.cn/gtbzrlipet.html

[T45] Perl：数组遍历
来源：http://hz.yongpay.top/gtrogytfls.html

for my $x (@arr) { print $x; }
来源：http://hz.tanke756.top/gtimgexvhf.html

[T46] Perl：哈希操作
来源：http://hz.zhaomingkeji.xyz/gtcwhdkowg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sxryk.cn/gtyvtkohtq.html

[T47] Perl：正则捕获
来源：http://hz.ydjk.org.cn/gtkyegelwt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hnxiangtu.top/gtlowfdflu.html

[T48] Perl：正则替换
来源：http://hz.yuanzhike.top/gtiqmthenq.html

$s =~ s/old/new/g;
来源：http://hz.pengpengdd.cyou/gtodeloiay.html

[T49] Perl：函数
来源：http://hz.zhengqikj.top/gtzdsiagdm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenlongwang.top/gtrsvzhlyq.html

[T50] Perl：逐行读文件
来源：http://hz.yuxming.cn/gttbdkpdjj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.guannengcc.top/gtnixfaorg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtfrtmqrlv.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtqcfevcfg.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtaljfaicn.html

[T52] Scala：变量
来源：http://hz.snrcjt.cn/gtlyeyntzo.html

val a = 1;  var b = 2
来源：http://hz.zhaomingkeji.xyz/gtawmgjsgg.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtvdlwisig.html

s"值: $b"
来源：http://hz.yangfankeji.com/gtffarithb.html

[T54] Scala：集合映射
来源：http://hz.guannengcc.top/gtrvvhklvm.html


<!-- 参考信息 -->