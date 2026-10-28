代发 wailian999

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtlleaqqzg.html

[R38] 管道串联
来源：http://hz.nwbrower.top/gttkqeynps.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cucudq.cn/gtodvmplie.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtdipdbvpf.html

cmd > out.log 2>&1
来源：http://hz.hnqzz.top/gtkejnjlaa.html

[R40] 追加写日志
来源：http://hz.cashguo.top/gtizuceefd.html

echo "log" >> out.log
来源：http://hz.yonumen.top/gtypkbzkgp.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtfmwsstuq.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtwvqcjuus.html

[R42] 输入重定向
来源：http://hz.yangfankeji.com/gtcbrsobpa.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gtnugheskl.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtirtashow.html

find . -name "*.log" -type f
来源：http://hz.jqgfzy.top/gtswepwxsb.html

[R44] 按修改时间查找
来源：http://hz.birdmap.top/gtnrjmaanh.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtpeikrjgd.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtkewjmwgj.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gtlpziivra.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gtkvhqyvau.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gogol.net.cn/gtzarglqhz.html

[R47] sed 单行替换
来源：http://hz.jlsjyb.cn/gtwmjpgzwu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtwinrflwa.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtsjvmeydf.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenlongwang.top/gtqlviljmk.html

[R49] awk 带条件
来源：http://hz.cheryme.top/gtufblkmph.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.svipenyu.cn/gtnjeffvgb.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtmvxagmrs.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gthkrqtvzv.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtzfqiqosu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gtlcgqbfjc.html

[R52] 统计行数
来源：http://hz.andypj.xyz/gtfyupntsc.html

wc -l a.txt
来源：http://hz.nwbrower.top/gtkpriqljj.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtxvvnjjzs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cqqwz.cn/gtlbmiuaot.html

[R54] 比较两个文件
来源：http://hz.iojbl.cn/gtkgmacgpk.html

diff a.txt b.txt
来源：http://hz.andypj.xyz/gtuwnnsibs.html

[R55] 压缩与解压
来源：http://hz.0kj1m.cn/gtlaptzzbj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gttunzodnp.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtfsmainqm.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gtrwvpfwvg.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtadsnvzqk.html

ssh user@host 'uptime'
来源：http://hz.jiagoushi.top/gtqokrocpd.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtrkfxltkq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sufxvd.cn/gtbkicgewm.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtifozrccf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhengqikj.top/gtbuipdkxf.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtlizvdxhc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gtcbluzkmj.html

[R61] 磁盘占用
来源：http://hz.ivvv.top/gtwaislxvv.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gttpwosabi.html

[R62] 找最占空间的文件
来源：http://hz.kuanghao11.cn/gteaqmmkfn.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtnxpjribw.html

[R63] 内存与进程
来源：http://hz.dianchejie.cn/gtozlzeils.html

free -h;  ps aux | grep nginx
来源：http://hz.316326.xyz/gtyfrgtwry.html

[R64] 结束进程
来源：http://hz.jlsjyb.cn/gtgwlyvbgh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gtxmnarvpg.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtyngbpdcd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtyrwsdolw.html

[R66] 定时任务
来源：http://hz.kuanghao11.cn/gtnuhrhkvu.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtsirmvmru.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtbfeqrbpo.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gteztlvryi.html

[R68] 计算文件校验值
来源：http://hz.gogol.net.cn/gtewcujzdt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtqwmfzyuc.html

[R69] 生成随机密码
来源：http://hz.fzhhl.top/gtpwbfkewt.html

head -c 16 /dev/urandom | base64
来源：http://hz.kuanghao11.cn/gtccakmaqq.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gtoihdqsll.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtddvewrdc.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtpohfxgrv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guannengcc.top/gtdnbgqhmp.html

[R72] 等待端口就绪
来源：http://hz.fzhhl.top/gtizirnunu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtoolswzcc.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gtpgejwzyj.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtixpkkpks.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtebnycxtx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhiwuduotai.top/gtdypaknbq.html

[R75] 导出环境变量
来源：http://hz.nwbrower.top/gtilelxvgf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guannengcc.top/gtxjcselzc.html

[R76] 使用临时文件
来源：http://hz.xziqi.cn/gtreheyyjk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtieokidni.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gtwsdfstyy.html

read -rp "请输入: " ans
来源：http://hz.sxryk.cn/gtyiawhnig.html

[R78] 交互式菜单
来源：http://hz.chenlongwang.top/gtzyogaxjo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhaomingkeji.xyz/gtggexnyxj.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtgyqteqyr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtexedgksc.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gthjayjgju.html

time ./run.sh
来源：http://hz.hysaishi.cn/gtrrrkeuno.html

================================================================================
来源：http://hz.bjfxy.top/gtamsbxnmn.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtqmdoupsr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtezujnsgv.html

[S01] C：Hello World
来源：http://hz.meibo888.top/gtagmlgotl.html

#include <stdio.h>
来源：http://hz.aizwys.cn/gtrzwfjnye.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtreqaurfy.html

[S02] C：变量与格式化输出
来源：http://hz.smart0.xyz/gtpojmweyt.html

int a = 10; printf("%d\n", a);
来源：http://hz.pengpengdd.cyou/gtzhvppapv.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gtyqbspwqf.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtofthtknu.html

[S04] C：字符串复制
来源：http://hz.xuetiantiany.cn/gtstlrrxxs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.316326.xyz/gtzvlwnmng.html

[S05] C：字符串长度
来源：http://hz.52xcode.cn/gtqtjlrjvc.html

strlen(s)
来源：http://hz.jqgufenzy.top/gtcadqwcjx.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtugypnsih.html

strcmp(a, b) == 0
来源：http://hz.hywenlv.cn/gtzaahqhmk.html

[S07] C：数组遍历求和
来源：http://hz.jlsjyb.cn/gtiridrjqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hywenlv.cn/gtcobfxxwp.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtivneqftx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dashuyun.cn/gtdihyoddu.html

[S09] C：结构体定义与初始化
来源：http://hz.ehwqpu.com/gtfojtbjab.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cashguo.top/gtnpjvwkbf.html

[S10] C：指针与解引用
来源：http://hz.sufxvd.cn/gtzyliwdot.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtmcsaohzm.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtgpifoacu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtmqedsrpm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jianghu66.top/gtdaftwvgc.html

fclose(f);
来源：http://hz.9152youxi.cn/gtithhzvso.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtyaphlcit.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.snrcjt.cn/gtoluldkvr.html

[S13] C：宏定义
来源：http://hz.yuxming.cn/gtlozaeaai.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.havefunace.top/gtkayaypdc.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtfmrmpijf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.52xcode.cn/gtuulljxfn.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gtwhfinfny.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtgvnzplpv.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gtwckegjzj.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtgycygjrs.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtbilgvvut.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xingfuxueyuan.xyz/gtzlchinxu.html

[S18] C：命令行参数
来源：http://hz.yuxming.cn/gtgqtmlela.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtxxjcqspv.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtadfzrzbj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gttrwukthh.html

[S20] C：二分查找
来源：http://hz.pycfn.com/gtpivkdguo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtndqbhlnd.html

[S21] C：字符类别判断
来源：http://hz.jyoumei.cn/gtwrvculbc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.meibo888.top/gtmsbntejh.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gtyvqkoemv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgufenzy.top/gtwsdmgsqw.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtxbxoifzh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sweek.top/gtzdxligjf.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gtzmtzvrnm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fzhhl.top/gtelykggib.html

[S25] C：内存拷贝
来源：http://hz.hnqzz.top/gtuiavpldk.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtanipppds.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtbeahdezi.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtdbuvsyrg.html

[S27] C：定义常量
来源：http://hz.zhixingplan.top/gtwesbqfbf.html

const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gtxyycjapi.html

[S28] C：静态变量
来源：http://hz.jqgufenzy.top/gtwcwqlikf.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtpercgzbw.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtstchztnr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gtczppwupj.html

[S30] C：头文件保护
来源：http://hz.meibo888.top/gtdobweamv.html

#ifndef X_H
来源：http://hz.316326.xyz/gtdqnjxhxj.html

#define X_H
来源：http://hz.jinghuilouyu.cn/gtflaewtai.html

#endif
来源：http://hz.xuanzx.com/gtsayfqpiw.html

[S31] C++：Hello World
来源：http://hz.redwolf501.top/gtdtzwslxa.html

#include <iostream>
来源：http://hz.aibaodan.cn/gtssvyygqt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ppjwa.cn/gthygfnttt.html

[S32] C++：字符串
来源：http://hz.52xcode.cn/gtxprczovw.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtibsljbag.html

[S33] C++：vector 增删
来源：http://hz.fzhhl.top/gtoccaqnzj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuanzx.com/gtupcdjrbb.html

[S34] C++：遍历 vector
来源：http://hz.guowangkeji.top/gtpecatzde.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.vqdsnc.cn/gtisxylgyp.html

[S35] C++：map
来源：http://hz.wangdashe.top/gtyrcbleal.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtkxpptmbk.html

[S36] C++：unordered_map
来源：http://hz.zdqjudy.top/gtlaaazupy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtovxecqmr.html

[S37] C++：set
来源：http://hz.hfpthk.cn/gtudyhcuru.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daria6918.cn/gtsexcmzoj.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtusohcqcu.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtgufjpmkw.html

[S39] C++：自定义比较器排序
来源：http://hz.yvedp.cn/gtumpcaoqo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gtwaqeyvte.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gtunnpxusy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gtwzmgukmv.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtltuxreat.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gzhubu.top/gtrjwyyozn.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gtvhewujek.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuanzhike.top/gtbtnbsufm.html

[S43] C++：智能指针
来源：http://hz.jinghuilouyu.cn/gtzldfzuqq.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydzc1.top/gtzmygvmsy.html

[S44] C++：引用传参
来源：http://hz.fzhhl.top/gtlhxcxuaa.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtqmodiayp.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtszrukogc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtznvompjs.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtrnhuinba.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yangfankeji.com/gtcdqszrky.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydjk.org.cn/gtdzvdwzhs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydzc1.top/gtabfjgcpi.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtnfqdfces.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhixingplan.top/gtxcwnufwf.html

while (std::getline(in, line)) { }
来源：http://hz.0kj1m.cn/gthxmcuqzm.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gthhwdnbjk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dianchejie.cn/gtasatupxd.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gtjlxfbout.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gtzpnsjtbk.html

[S51] C++：显式类型转换
来源：http://hz.redwolf501.top/gtkdyrnwvs.html

static_cast<double>(a) / b
来源：http://hz.zycfv.cn/gtzgxuzzrh.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gtpeikxchk.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtsscieqfv.html

[S53] C++：移动语义
来源：http://hz.guowangkeji.top/gtigpasqaw.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gtqaeicrhy.html

[S54] C++：异常处理
来源：http://hz.bjfxy.top/gthiqxtmja.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gtntdmpocd.html

[S55] C++：结构化绑定
来源：http://hz.dianchejie.cn/gtpqlzanmu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtxngvzweo.html

[S56] C++：optional
来源：http://hz.zhoulong.xyz/gtpnsexcss.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pengpengdd.cyou/gtlrospbao.html

[S57] C++：编译期常量
来源：http://hz.chenzaomai.com/gtelmpctit.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtmcwduylm.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtsiatpwjx.html

namespace ns { int f() { return 1; } }
来源：http://hz.hfpthk.cn/gtksdrylxj.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtlvmixfrt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.havefunace.top/gtfapzqnhz.html

[S60] C++：遍历并删除元素
来源：http://hz.zycfv.cn/gtfbanktlf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ivvv.top/gtdhaoythw.html

================================================================================
来源：http://hz.xinyue.icu/gtmbqopgqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtmitwbjmg.html

================================================================================
来源：http://hz.jqgfzy.top/gtirnbkxkh.html

[T01] Kotlin：Hello World
来源：http://hz.fzhhl.top/gtmhbyutpz.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtcgjegjbw.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtclqfxqcr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cdnleiting.top/gtucnibnmx.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtivccyknn.html

"值: $b"
来源：http://hz.yanxiufei.cn/gtnjhhfegv.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtiudslofe.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gteexfgykf.html

[T05] Kotlin：when 表达式
来源：http://hz.xingfuxueyuan.xyz/gtgtmjaoog.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.nanxuanxn.top/gtpboxcdzr.html

[T06] Kotlin：集合映射
来源：http://hz.kuanghao11.cn/gtmxelueya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.andypj.xyz/gtexejtsbv.html

[T07] Kotlin：集合过滤
来源：http://hz.svipenyu.cn/gtsdaazjad.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuetiantiany.cn/gtlwcpybot.html

[T08] Kotlin：数据类
来源：http://hz.hammf.cn/gtpuivznjo.html

data class User(val name: String, val age: Int)
来源：http://hz.hnxiangtu.top/gtlxqydqqp.html

[T09] Kotlin：扩展函数
来源：http://hz.zhixingplan.top/gtnuttatmi.html

fun String.exclaim() = this + "!"
来源：http://hz.hnqzz.top/gtbustmpbh.html

[T10] Kotlin：默认参数
来源：http://hz.jianghu66.top/gtbvngoace.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hfpthk.cn/gtjlyqnahn.html

[T11] Kotlin：协程
来源：http://hz.nanxuanxn.top/gtxncklgjw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jlsjyb.cn/gtthilvefk.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtxhsdcbwj.html

val (a, b) = Pair(1, 2)
来源：http://hz.guannengcc.top/gtftudhcpb.html

[T13] Kotlin：只读 Map
来源：http://hz.zhaomingkeji.xyz/gtqvuasfvh.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtyiiucvzx.html

[T14] Kotlin：循环
来源：http://hz.jinyuanbaomall.cn/gtggsvzwip.html

for (i in 1..10) println(i)
来源：http://hz.hnqzz.top/gtrtrxpghw.html

[T15] Kotlin：接口
来源：http://hz.sufxvd.cn/gtpzftspla.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtiqjnrqso.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtwubsvkyl.html

print("Hello")
来源：http://hz.chenlongwang.top/gtyakfpsci.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gtfafwewwc.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtovhdwock.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtwpeydddv.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtrvvqalzy.html

[T19] Swift：可选绑定
来源：http://hz.hammf.cn/gtxtuoauxl.html

if let n = opt { print(n) }
来源：http://hz.birdmap.top/gtohobjeqh.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gtegbovzoc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shangyingyoupin.top/gtyavsqznq.html

[T21] Swift：遍历
来源：http://hz.cheryme.top/gtxvcndzdz.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtkgzvzfwl.html

[T22] Swift：字典
来源：http://hz.cheryme.top/gtdolyokle.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj20258.top/gtlkogulzn.html

[T23] Swift：函数
来源：http://hz.yangfankeji.com/gtiwizbhvg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zycfv.cn/gtjrolgccx.html

[T24] Swift：闭包
来源：http://hz.xinyue.icu/gtbialopnx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shzxlz.cn/gtqnpfceqe.html

[T25] Swift：结构体
来源：http://hz.cheryme.top/gteluxrjev.html

struct P { var x: Int }
来源：http://hz.yongpay.top/gtojayajcz.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtiqoqukao.html

class A: Base { override func f() {} }
来源：http://hz.zdqjudy.top/gtbkesnmwd.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtudwbbayw.html

do { try f() } catch { print(error) }
来源：http://hz.daxiang520.top/gtmnjzbpja.html

[T28] Swift：枚举
来源：http://hz.9152youxi.cn/gtcstspolw.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtodeakcnm.html

[T29] Swift：guard 提前返回
来源：http://hz.pengpengdd.cyou/gtdsibglze.html

guard let x = opt else { return }
来源：http://hz.zycfv.cn/gtvynqmfwg.html

[T30] Swift：协议
来源：http://hz.tian-w.cn/gtdmntjbuw.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtmreliaqa.html

[T31] Lua：Hello World
来源：http://hz.0kj1m.cn/gtweumihih.html

print("Hello")
来源：http://hz.yj202588.top/gtjmdqcaea.html

[T32] Lua：局部变量
来源：http://hz.tian-w.cn/gtjykddeph.html

local a = 1
来源：http://hz.kuanghao11.cn/gtvzmtdocn.html

[T33] Lua：表（数组）
来源：http://hz.yangfankeji.com/gtsxpqnvba.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.fengsongda.top/gttzjduuxa.html

[T34] Lua：遍历表
来源：http://hz.tanke756.top/gtmfbjyjmz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.andypj.xyz/gtvxbkegtv.html

[T35] Lua：字典表
来源：http://hz.jyoumei.cn/gteqgfvide.html

local d = { a = 1 };  d.b = 2
来源：http://hz.quarkkingdee.top/gtucumowib.html

[T36] Lua：函数
来源：http://hz.jinqigufen.top/gthhkntfsw.html

function add(a, b) return a + b end
来源：http://hz.hysaishi.cn/gtjgmzakyb.html

[T37] Lua：字符串拼接
来源：http://hz.sweek.top/gtyzefncnx.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtnbqsshee.html

[T38] Lua：条件
来源：http://hz.shuidangran.top/gtrqtrcgdd.html

if x > 0 then print("正") end
来源：http://hz.xylfe.cn/gtsolyvfqw.html

[T39] Lua：模式匹配
来源：http://hz.vqdsnc.cn/gtrkruyero.html

string.find(s, "%d+")
来源：http://hz.yj20258.top/gtiihfojfu.html

[T40] Lua：元表
来源：http://hz.guannengcc.top/gtdyongedv.html

setmetatable({}, { __index = base })
来源：http://hz.cqqwz.cn/gteigrgzpb.html


<!-- 参考信息 -->