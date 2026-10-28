代发 wailian999

find . -name "*.log" -type f
来源：http://hz.shanyushiyangtech.top/gtclvwfmzb.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtaevpkycg.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtjfsirltx.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtbeuxumzf.html

find . -name "*.tmp" -delete
来源：http://hz.hammf.cn/gtkvotkkeu.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtlvcrepds.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xylfe.cn/gtwfvgqbyb.html

[R47] sed 单行替换
来源：http://hz.jianghu66.top/gtabmryqbh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangshuangyany.cn/gtqbmpojdd.html

[R48] awk 取指定列
来源：http://hz.gzhubu.top/gtwfpdqcyf.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangtech.top/gtzzthctyz.html

[R49] awk 带条件
来源：http://hz.hnxiangtu.top/gtetiidufy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sweek.top/gtjenyncvq.html

[R50] awk 求和
来源：http://hz.yvedp.cn/gtcmrwgmqn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenjidiqi.icu/gtzhwxwyew.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gtqomyrmpq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtmwbiagoc.html

[R52] 统计行数
来源：http://hz.fengsongda.top/gthmemspjz.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gtoudpwkkr.html

[R53] 查看文件头与实时尾
来源：http://hz.jlsjyb.cn/gtoddpgoni.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gthljdefnf.html

[R54] 比较两个文件
来源：http://hz.iojbl.cn/gtejbzkbtc.html

diff a.txt b.txt
来源：http://hz.aizwys.cn/gtpmydnurv.html

[R55] 压缩与解压
来源：http://hz.ydjk.org.cn/gtxbffuxtk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hysaishi.cn/gtkhnjbpsn.html

[R56] 远程拷贝
来源：http://hz.jlsjyb.cn/gtehnyogon.html

scp file user@host:/path/
来源：http://hz.jianghu66.top/gtbtgcqfnu.html

[R57] 远程执行命令
来源：http://hz.daxiang520.top/gtowcgcraa.html

ssh user@host 'uptime'
来源：http://hz.sysykeji.top/gtchbosfmd.html

[R58] 下载文件
来源：http://hz.zhaomingkeji.xyz/gtfyogeixw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258888.top/gtmuiwlhbk.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtlmysttsy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtkzxuwmoo.html

[R60] 只看 HTTP 状态码
来源：http://hz.zdqjudy.top/gtwzqrhidf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuanzx.com/gtqworqjpi.html

[R61] 磁盘占用
来源：http://hz.yangfankeji.com/gtqzexijkk.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtkeykojyr.html

[R62] 找最占空间的文件
来源：http://hz.dashuyun.cn/gtnrekugep.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxuanxn.top/gtkynyeqfd.html

[R63] 内存与进程
来源：http://hz.hnqzz.top/gthbbjzcgs.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtuhacjepv.html

[R64] 结束进程
来源：http://hz.yangfankeji.com/gtwyoifzkf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtmpjofdpq.html

[R65] 查看端口占用
来源：http://hz.316326.xyz/gtxqjnebqm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tanke756.top/gtxokxuxau.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtvsheqmub.html

crontab -e;  crontab -l
来源：http://hz.xziqi.cn/gtwpfmtwrz.html

[R67] 生成随机十六进制串
来源：http://hz.zycfv.cn/gtiiwprqdu.html

openssl rand -hex 16
来源：http://hz.hysaishi.cn/gttlswayur.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtqngotfxl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gtqwxwralr.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtwumzrihr.html

head -c 16 /dev/urandom | base64
来源：http://hz.sxryk.cn/gtytoxchqm.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtdmotazve.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtlutndjfl.html

[R71] 日期格式化
来源：http://hz.iojbl.cn/gtkcxevigv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenjidiqi.icu/gtzuwihfxz.html

[R72] 等待端口就绪
来源：http://hz.shuidangran.top/gtkowcmgmu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtgaxistpn.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gthpdwzjxo.html

split -l 1000 big.log part_
来源：http://hz.guannengcc.top/gtdcypiske.html

[R74] 批量重命名
来源：http://hz.gzhubu.top/gtwiqohoiu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dashuyun.cn/gtpigobphe.html

[R75] 导出环境变量
来源：http://hz.yj202588.top/gtrjsrdkpk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinghuilouyu.cn/gtnmvvfjkq.html

[R76] 使用临时文件
来源：http://hz.pengpengdd.cyou/gtfpamfdwj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtifkdvaxw.html

[R77] 读取用户输入
来源：http://hz.zdqjudy.top/gtiqpnuhxy.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtdsbrwcaq.html

[R78] 交互式菜单
来源：http://hz.zhoulong.xyz/gtuewhmjua.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xylfe.cn/gtfvorwsqk.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtimjstbww.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gtvzwmlqxc.html

[R80] 查看脚本执行耗时
来源：http://hz.ydjk.org.cn/gtambqgndt.html

time ./run.sh
来源：http://hz.yj20258.top/gtajozmtgo.html

================================================================================
来源：http://hz.zhixingplan.top/gttwmqsdev.html

S. C / C++ 专题
来源：http://hz.dianchejie.cn/gtjsqrubpl.html

================================================================================
来源：http://hz.andypj.xyz/gtqqgpkewg.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtcrburwks.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtxummbcdv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtnblgkfcz.html

[S02] C：变量与格式化输出
来源：http://hz.xinyue.icu/gtmvfqdgah.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258888.top/gtkhnvjrdk.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtyqlnovbt.html

int x; scanf("%d", &x);
来源：http://hz.cucudq.cn/gtpbucgfog.html

[S04] C：字符串复制
来源：http://hz.dianchejie.cn/gtvakkzfbo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daxiang520.top/gtellquhqb.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtqqsnyyaz.html

strlen(s)
来源：http://hz.smart0.xyz/gtryzqueza.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gtxdizfsse.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtjtsbizve.html

[S07] C：数组遍历求和
来源：http://hz.hysaishi.cn/gthjhebfnv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gtcljhobxk.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gthrftlvyz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtbgwnnwfp.html

[S09] C：结构体定义与初始化
来源：http://hz.yuanzhike.top/gtchmeginh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtoizizkik.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gttwgftteh.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtilmihptw.html

[S11] C：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtnnscqafi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtmynpsudb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtzlmtcedd.html

fclose(f);
来源：http://hz.yueranfly.top/gtfktvyqiu.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gtlroaawtd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtcrjchyjf.html

[S13] C：宏定义
来源：http://hz.xingfuxueyuan.xyz/gtuxgikmkn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pycfn.com/gteyfoqkak.html

[S14] C：枚举
来源：http://hz.meibo888.top/gtpijtfdcw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.meibo888.top/gtabhobsgp.html

[S15] C：类型转换
来源：http://hz.hnxiangtu.top/gtdfddboey.html

(double) a / b
来源：http://hz.fzhhl.top/gtbyvhnttu.html

[S16] C：位操作置位
来源：http://hz.svipenyu.cn/gtueluwelx.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtunggezwu.html

[S17] C：安全拼接字符串
来源：http://hz.9152youxi.cn/gtwthmgvvz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shangyingyoupin.top/gtktxnfqvu.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gtvbouabdl.html

int main(int argc, char **argv)
来源：http://hz.yanxiufei.cn/gttwqgmpag.html

[S19] C：快速排序
来源：http://hz.dianchejie.cn/gtjbmfiknp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtrqllstkb.html

[S20] C：二分查找
来源：http://hz.jinyuanbaomall.cn/gthcxqzywm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtttpjypre.html

[S21] C：字符类别判断
来源：http://hz.svipenyu.cn/gtpgzdxtxb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtqypcjqtx.html

[S22] C：字符串转数字
来源：http://hz.tianlin.xyz/gtqrdcgvpj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jiagoushi.top/gtfktwwfnb.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gtupdfyjfn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtyoscniqc.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gtgpdhjosv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtmvoxcnbh.html

[S25] C：内存拷贝
来源：http://hz.jqgufenzy.top/gtlqczbjje.html

memcpy(dst, src, n);
来源：http://hz.jinghuilouyu.cn/gtfsphucsl.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtewmcnohe.html

memset(a, 0, sizeof a);
来源：http://hz.cashguo.top/gtgmvdxubx.html

[S27] C：定义常量
来源：http://hz.haohaochexian.top/gtyyimpaum.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtnjofnnkk.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtlqcinwmw.html

static int counter = 0;
来源：http://hz.jianghu66.top/gtalcnwvee.html

[S29] C：变参函数
来源：http://hz.pengpengdd.cyou/gtibsrroii.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtfyvqpjyq.html

[S30] C：头文件保护
来源：http://hz.ivvv.top/gtynmucawr.html

#ifndef X_H
来源：http://hz.gzhubu.top/gtlydlywgx.html

#define X_H
来源：http://hz.hysaishi.cn/gticrhzxke.html

#endif
来源：http://hz.jqgufenzy.top/gtdclkntfy.html

[S31] C++：Hello World
来源：http://hz.nwbrower.top/gtereykfuv.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtbrxvrydu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fzhhl.top/gtfiyvesui.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtelexfeta.html

std::string s = "hi";  s += "!";
来源：http://hz.chenlongwang.top/gtvnffifbg.html

[S33] C++：vector 增删
来源：http://hz.quarkkingdee.top/gtglyxlada.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xziqi.cn/gtkoqcczou.html

[S34] C++：遍历 vector
来源：http://hz.aibaodan.cn/gtfzxpxqqn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shzxlz.cn/gtpaehewwa.html

[S35] C++：map
来源：http://hz.gotoacloud.top/gtkklylsdj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtilvqnpuv.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gttrboflwa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtkvuohdcy.html

[S37] C++：set
来源：http://hz.cashguo.top/gtbtcaizfd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtqfmvqcvj.html

[S38] C++：排序
来源：http://hz.daxiang520.top/gtwecluhhh.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgfzy.top/gtnpkfseav.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtxwxhlayf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydjk.org.cn/gtzuwtwwaz.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtjtkckndl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daria6918.cn/gtocwvrptq.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtduuzhfdl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.316326.xyz/gtcvmxwamz.html

[S42] C++：继承与虚函数
来源：http://hz.gotoacloud.top/gtodgbjqkt.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenlongwang.top/gtrldjneux.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtcmfbiuop.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtufjqsofy.html

[S44] C++：引用传参
来源：http://hz.jinyuanbaomall.cn/gtdtvfudlw.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gtrqofljdc.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtcqwuwzor.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxinkj.top/gtsmrrosax.html

[S46] C++：函数模板
来源：http://hz.ybcxt.top/gtomksuifo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.svipenyu.cn/gtnqtkifda.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gtipvaftaq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtbouhvxgr.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gteosmscdp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.bjfxy.top/gtyhwgslwj.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gtwnznlong.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtxtxepnqu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gtmdmsouwt.html

[S50] C++：格式化数字
来源：http://hz.tanke756.top/gtezgottla.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhoulong.xyz/gthjlhzkec.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtbhzofwiu.html

static_cast<double>(a) / b
来源：http://hz.daxiang520.top/gtcfqoaezq.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxinkj.top/gtojiccian.html

int size() const noexcept { return n_; }
来源：http://hz.cashguo.top/gtkufxjzha.html

[S53] C++：移动语义
来源：http://hz.sweek.top/gtpnnfeivf.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtmjtfosrp.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangtech.top/gtpgaflvfk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.haohaochexian.top/gttpydrtwl.html

[S55] C++：结构化绑定
来源：http://hz.tianlin.xyz/gtmmrbvbus.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtdrxgryfu.html

[S56] C++：optional
来源：http://hz.hnxiangtu.top/gtpiiacyyg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yonumen.top/gtbifwrjbs.html

[S57] C++：编译期常量
来源：http://hz.jqgufenzy.top/gtoxgvayxw.html

constexpr int N = 10;
来源：http://hz.shzxlz.cn/gtvqcexnqp.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gtukrssfvp.html

namespace ns { int f() { return 1; } }
来源：http://hz.snrcjt.cn/gtcnheuufw.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtbojxsecx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gttgfazuow.html

[S60] C++：遍历并删除元素
来源：http://hz.ybcxt.top/gtqwwueyat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aibaodan.cn/gtvirebtaq.html

================================================================================
来源：http://hz.redwolf501.top/gtzghpftmf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtrnkngucc.html

================================================================================
来源：http://hz.hfpthk.cn/gtfgfqasqn.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtswrpzgcc.html

println("Hello")
来源：http://hz.zhengqikj.top/gtnmlfabfk.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtbwerjjbx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtjiybdnye.html

[T03] Kotlin：字符串模板
来源：http://hz.birdmap.top/gtkoncwkzv.html

"值: $b"
来源：http://hz.bjfxy.top/gttxzituor.html

[T04] Kotlin：空安全
来源：http://hz.yj202588.top/gtptllvumo.html

val n: String? = null;  n?.length
来源：http://hz.sufxvd.cn/gtwhtfphtm.html

[T05] Kotlin：when 表达式
来源：http://hz.aizwys.cn/gtdstedqou.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fzhhl.top/gtidtnvgsd.html

[T06] Kotlin：集合映射
来源：http://hz.hfpthk.cn/gtnjagqxsn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangkeji.top/gtqtoefzpo.html

[T07] Kotlin：集合过滤
来源：http://hz.yanxiufei.cn/gtxvnvnifd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuxming.cn/gtushnqpnl.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gtarwpgzgx.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtfhmbfffl.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtiyrwaqvw.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtazwgtlfq.html

[T10] Kotlin：默认参数
来源：http://hz.hfpthk.cn/gtxkoymmyw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydjk.org.cn/gtkedwtyff.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtudrmtnnz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gotoacloud.top/gtfybvtpof.html

[T12] Kotlin：解构声明
来源：http://hz.52xcode.cn/gtxzkgebme.html

val (a, b) = Pair(1, 2)
来源：http://hz.52xcode.cn/gtsygygkfy.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258888.top/gtqanicdqv.html

val m = mapOf("a" to 1)
来源：http://hz.xinyue.icu/gtpbeyekbm.html

[T14] Kotlin：循环
来源：http://hz.ydjk.org.cn/gtlicupdlx.html

for (i in 1..10) println(i)
来源：http://hz.9152youxi.cn/gtkbtujlaf.html

[T15] Kotlin：接口
来源：http://hz.jyoumei.cn/gtnxarkchq.html

interface Shape { fun area(): Double }
来源：http://hz.snrcjt.cn/gthxegpohg.html

[T16] Swift：Hello World
来源：http://hz.cdnleiting.top/gtllkhaplr.html

print("Hello")
来源：http://hz.gotoacloud.top/gtxsdqzfpl.html

[T17] Swift：变量与常量
来源：http://hz.zdqjudy.top/gtsofmwkbq.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gtzispgqca.html

[T18] Swift：字符串插值
来源：http://hz.chenlongwang.top/gtjbawjkge.html

"值: \(b)"
来源：http://hz.redwolf501.top/gtsvcofkps.html

[T19] Swift：可选绑定
来源：http://hz.tianlin.xyz/gtfxsocebd.html

if let n = opt { print(n) }
来源：http://hz.dashuyun.cn/gtuhyndhmt.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtmexcpgpm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gtkbilbxwa.html

[T21] Swift：遍历
来源：http://hz.hysaishi.cn/gthiodthwp.html

for x in a { print(x) }
来源：http://hz.hnqzz.top/gtzvwfastb.html

[T22] Swift：字典
来源：http://hz.yonumen.top/gtjqnlyotk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.smart0.xyz/gtbbwwjvtt.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtprgngcri.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangdashe.top/gtmancmbmc.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtcnqjwllp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tanke756.top/gtpjcoqwbw.html

[T25] Swift：结构体
来源：http://hz.shangyingyoupin.top/gtmeexjmrj.html

struct P { var x: Int }
来源：http://hz.ydzc1.top/gtxkkshtzf.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtygqtuzbx.html

class A: Base { override func f() {} }
来源：http://hz.hfpthk.cn/gtpahqbwrf.html

[T27] Swift：错误处理
来源：http://hz.sysykeji.top/gtredwlhin.html

do { try f() } catch { print(error) }
来源：http://hz.daria6918.cn/gtefzzvuaa.html

[T28] Swift：枚举
来源：http://hz.zhengqikj.top/gtrwaditrd.html

enum Color { case red, green }
来源：http://hz.yongpay.top/gtgpwrcgpn.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gtvbggnhoh.html

guard let x = opt else { return }
来源：http://hz.jinyuanbaomall.cn/gtesqrctum.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtladaoxnw.html

protocol Shape { func area() -> Double }
来源：http://hz.gaohongyu789.top/gteyhlksha.html

[T31] Lua：Hello World
来源：http://hz.yongpay.top/gtkvhxpohi.html

print("Hello")
来源：http://hz.nwbrower.top/gtesmvncqe.html

[T32] Lua：局部变量
来源：http://hz.xuanzx.com/gtcbxdxxyh.html

local a = 1
来源：http://hz.hysaishi.cn/gtihdismpy.html

[T33] Lua：表（数组）
来源：http://hz.yj202588.top/gteonvmcme.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daria6918.cn/gtojgmgjlp.html

[T34] Lua：遍历表
来源：http://hz.shzxlz.cn/gtpmchmtxa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.birdmap.top/gtrqljwcbx.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtmzuhuqwp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.c1oappe.top/gtpqidjomd.html

[T36] Lua：函数
来源：http://hz.zhaomingkeji.xyz/gtycmcpmss.html

function add(a, b) return a + b end
来源：http://hz.aibaodan.cn/gtqlxigwdm.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtytibyflm.html

"a" .. "b"
来源：http://hz.fengsongda.top/gtwzfiecyw.html

[T38] Lua：条件
来源：http://hz.quarkkingdee.top/gtsvfcdmpp.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gtzlhmrmkl.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtfqehikmi.html

string.find(s, "%d+")
来源：http://hz.gzhubu.top/gtehfdgbhn.html

[T40] Lua：元表
来源：http://hz.quarkkingdee.top/gtisphyuom.html

setmetatable({}, { __index = base })
来源：http://hz.nanxuanxn.top/gtxvyrcymn.html

[T41] Perl：Hello World
来源：http://hz.xylfe.cn/gtgzukcuow.html

print "Hello\n";
来源：http://hz.jinyuanbaomall.cn/gtthlnelsh.html

[T42] Perl：变量类型
来源：http://hz.guannengcc.top/gtbqbhreqo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhengqikj.top/gtcumuktcm.html

[T43] Perl：字符串插值
来源：http://hz.hysaishi.cn/gtneuibjya.html

"值: $a"
来源：http://hz.chenlongwang.top/gtiphgsgej.html

[T44] Perl：条件
来源：http://hz.52xcode.cn/gtbsuagilv.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangkeji.top/gtqmpqpxll.html

[T45] Perl：数组遍历
来源：http://hz.yongpay.top/gtibelcrib.html

for my $x (@arr) { print $x; }
来源：http://hz.hammf.cn/gteyggkfdz.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gtvseocpcg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhongyouzk.top/gteinsgfis.html


<!-- 参考信息 -->