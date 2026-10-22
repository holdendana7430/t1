代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zwhlglur.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fuuwfaud.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2syyfisgo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ycsdrnvg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2bqqvtcnn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bvwkexkb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mfsyteyi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lkddhilj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyjfckch.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ffzhhjor.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vwdjwcfr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ghrosifa.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rxyxrxtt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xotgcafu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pbpoxalf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wfvqjzra.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uecqdqru.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hkeqlvsv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xxxquoin.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jspphkzn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bhqpzoid.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gkidmknw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xabzgcnw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2azwtrkrc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vnuszdkh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2krgspopf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uprnkbkp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qbgfbgve.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wdlbfddp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2labbnuxp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cctlkkii.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2sgtvgkio.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vwnbjzqd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xwkayaer.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lccbetgl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lxbgycjb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ifoqrfao.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mkzamloy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kqpexdpq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xlazgmlz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2szjtbpmu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bcenfbiw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jktutlom.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2poaselkv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uhdtlvmv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2myvbfxvy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gdgvyfdx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zsatddye.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pbgnacov.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jloievbk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2flezxdry.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dwdfsrqg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2aucuzcpr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jtnswusp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zulxqavb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xokpvjsb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nnhrmrvu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2erbbtesw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2yqydkhwy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rwzsywja.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2uxcfffxx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kzruclup.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qnnufbyo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lbepcuiy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wgwtxjyn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gyogbzko.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dknznstq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ntmyydej.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2knnzppnl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tfohtihq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2sthiufdy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fkqdmnrm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2occpqfmy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vyuiukoo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2psuxpefv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jzbclmuh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kvjvagjw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nwuvppgp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdbgctxn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vubstpff.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wxvkmash.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2yjsqgvby.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vqshmtah.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfecnitj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kqbcnhsp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcmrmxvr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xmtekzng.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dvwheqca.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2noziwwix.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wpekrkct.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2miwmoiyh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wuyrukmm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2budcditd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qxmlheuq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2czietezx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxqjrnif.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fqqarron.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grlgfwje.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2frakmzva.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lzquzozw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2euhshogm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lddvnfqd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rxdjhjxb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wuqzoqga.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2czzzfgcc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zxrfielo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mzswemdu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ptkfvsyj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pgyhxlkn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gjphmwjf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kzhfkvky.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gsxhbpjw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ysstnubq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2saqcewsh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yqnnxwzn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qqszfnvf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zxjpnkfw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2bpnrgkyj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dbkvpsne.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2llrueyoy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zbfnwssw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2occgpazd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cfozokzb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qferjyus.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zqujzoyu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ykipcdlc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qjydhtcg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mfgopsxt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kjfmovdd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bdxotncs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zrobkkrx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2woaizzji.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hznnijew.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qbvrftvp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gpzoucih.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sxxsemhd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2smlsefef.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2euuczqtq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pwlisaoy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jawtrzii.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rgwaooar.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2czsioxir.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tehdrmhp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2caaasgeh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2uqflwojl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zxtaerod.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cqsmolmt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ythtvgml.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rsnedzvb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ojvkgeiq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mgeepjgc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xzpxdxyu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gbgbdqbr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2chilnpcl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eyehaplx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nqatjwhx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zdtjcxlb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2feoknzmf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gpjauxer.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2eybyuqnr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pobhpcir.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gyjnjhrs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ysadnwuw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wwsrzakm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ugnzvaqo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkywivoy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hfqosrbb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zajzytru.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qhsjkjlc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ryxasxyl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2myiexrvk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2sqmphcfe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wbnfjjot.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mtjcmqdv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lkxjqrmw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojgyfidq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gknwmtoq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rpwhxqlo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aoeolxtt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2stndzksi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qhtqjqjy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vpccdwzc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nkirezdk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kzwppjaf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2szvyhocd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2bapsrfgj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2umkpvwvt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dgktyvlf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2avvqtkyo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yttgjhko.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2syghgdjo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nggknbbp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2byjfvirn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2iqetgnbi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pzsvnooz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilwasnev.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2shehloht.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuksksxf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qptnjhhg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ancnzbhe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2njcoaaki.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2immglxvt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2swpjfoxk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fshwxwdk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pglizski.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2svzbbjid.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kcjkkekt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bojaomzm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cchlyrga.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ybenxfnz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cjchgtjr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zgljvepa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2udyebrny.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fbudeojp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fajmbvyz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ndwyonvw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kblzzopc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2enusyxba.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jkllnwgo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qwzsmlcl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrscdxr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jkftvgxs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bzdzrkwa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xckuovtv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jdyjkcfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wquxnbqk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mkfoudfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjxkwckc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hihoascz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gijmvtlb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hytkmonl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2opwhnpop.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2svqyuthw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rgdqaqpi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ilxopbje.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pgaxojfn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mgsweraq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yfaoaqhk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jqgswztp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xifgveqi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lrgofure.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uzfswpen.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qvflqumv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ojsvyhvo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2msjatadp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gsiduvpl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bymrjogz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hupaxrkf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2orzouedh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2msadnvsb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xgkufhjw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsdfflr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lszjqnqp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hoedslzl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2viyhcwdf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wvlasnwr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hoigpcdj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2odagebtk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycxcnjss.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iflhtepl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2owivufqh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kqhewmmm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kaxauhkq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2acfdlyla.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vdaixnqd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jiikiogi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ttaaieoi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2cxmstdvr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rseocfxl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvyevwlo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lpemqmlp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ocraqzgz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmqhgjkl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ewqxxfec.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ukbtshuj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vysxxvkw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2arokgiqx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2izvignfc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fzvpgvbw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2myrhelta.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ivzdhwfg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yhbstbll.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pzmqnkuq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vifqxvvc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yrgejwur.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bynssebs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2egkphsdv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xzheaiar.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fsjpovur.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mmsysgcr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tqnhahfz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xhepiszf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2giwljezj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2otyedvgf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jbwqbmhr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cdncmyrl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jyfjeozn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vjzwgxol.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jfgwuwtl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aeudaohy.html


<!-- 参考信息 -->