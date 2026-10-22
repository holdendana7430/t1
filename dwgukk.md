代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ekbwzwbm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ocyhwbqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnmtzfos.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2acilqhzc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hbfuvbai.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ozizifzj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ymzqmkym.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ozwbgxte.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qjmuvgxp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tbfcjstq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qfwebssi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ewfgvtuw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2uckhasfn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jvfdqmpt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2axupwfqz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fmniuzyo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2oglgstml.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jjdwaaag.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kkcyvlsl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2atasgqns.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tonnnzgk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2njdvzbde.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2luyxhrfr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bzyxlwiw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lpfpqyhw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gbgysqhz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tbhdihft.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2astgyabb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jjmnfuwh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vmpxqsuj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lvkcdpzx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fdootiiv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2poymewem.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nkfpikeh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ibjspexu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hvjncbmb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ubkmbpga.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ajinzknl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jypaqyjn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tqnedxrv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cylupgsq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zdiwspyg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yitoxdpv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bjrcoizr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2grhvxwhw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pasxgjyn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtobgwcz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bqbziqmr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ielkqkqn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jlvlqaxg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vcmqqlci.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dmippfkn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sfuevfwc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tpfjeygx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2poymswnm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uojshkro.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jovfovjj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sksjuyol.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tghmliqj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2empvfusc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2srfxyzkb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xqpsgbry.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rzxfrjzu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dthsbyym.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2putwgofa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hdvfuhps.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wxqwavgw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hzftroaq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kgcxmvpu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nxyzgzzj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wjfhonxa.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vimxhcbp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2stspplgo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hofenjzg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2atuxnmxh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nfncvldk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2srvrejyn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pewzmvyo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ofpewcyk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vhvtysyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zcbgkxbq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vyfidgqn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2redfwzmc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2myvycvxw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hbvcznyv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2aewfrwqg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ecvpcymw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kcrrzfio.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hdxmxzdb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zbjlwyja.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kczkoozn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cdssfeul.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ghzhsuqd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ppguqwcs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2umnxccdc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qmdsispe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2pzhumbit.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2aqgqvpxe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wteaxahv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwomhzui.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vnceymvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anqgoxpl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sspqznvq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xjuunaia.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmzqmutr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uvjhukgj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2louiehgr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dcqhfpse.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hvogmmge.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zokbrvmm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tcidsvcw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qyjkifrx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tnbkjlgn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yzlthrhr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rxlkdrwe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qcwxniyl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yzljrhek.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uxryakfr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2gzqwdxqg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jxfhhlec.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kpmossyo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vuwghixv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2awhedeos.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mepohpte.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nhstdkqz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bjdhfxaa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cgoxpzwi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbghtyih.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gjzferhe.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2eyvzenhc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cosvekwq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ajlqryrw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zslrswbp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jmnzmzpw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2quqvqaxh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mucrhteg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2onqziexr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zgvgucmg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2aywcakve.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qwfyvita.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrorgsv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nmkibdzc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pobgtdab.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2iwwhgpnt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cotcwkzb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2pgkzxesy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ecvxibty.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lrnvzakn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ppggrooo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cjzkxmye.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mlluhbyl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2sbselpjh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ovvafbqm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yqcpyoow.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ubcgizos.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2olqsniob.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ngcgwdxt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zfdngdvb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kwwbdvkp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jswglwyu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zozimesc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mjqmcyvw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mlrfaqgq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jyameukq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cxkatfrb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uwxddyml.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2akpfevbb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qcquumce.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vytlaifj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wtxizcox.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2crvnlnzq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yeszcilw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wfucgpox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ytucpbdd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2eeewqufp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ozaaqkew.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fcrqtrrx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qcmmbqzn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ucecyzoq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rttjpuye.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wxfzcmja.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cbdrtxjg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tfyncnfa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fsowwcrt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tdwuuehu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2iteachev.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xqveasnn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hevbhhlr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2egwobkrl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hyuivirf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hnegaeyc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ljlhewcm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xmvpzlfs.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yktzfehd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2kqiuftbj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hmmjcdvl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fhtjrowe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qmpldppp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2plhudwgz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2epxuroee.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sdsbzpqq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ngxqzucq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kxsdbnjn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jkvfvejl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nfcubfra.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qturfdbe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2iiglrgfa.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gityuouh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pleujkdw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gacofbsa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nzcnsjkj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cmorxpjl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmnavqjr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2whxdclat.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2glqpznxl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mvtyaogf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lclqodbt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2krbczqmt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jajixyrp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2povkjqce.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yurublpy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2aezlkpkt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gjgqfzdo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vvibomhe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mrzvudeu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2leuualiv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zkwxgkzg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vybhsenm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2etympked.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhftxxxt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ktguxsmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glupilhy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sbquwlwq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bglwkrgc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wjozbptt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nmpfjijp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ttsdylyk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uezgjevb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hlasxdwx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tujnmohb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bywwpwez.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zrhvabmp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nxpsctwj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dwsndizk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kllixtdc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hbgsyqyn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tzgqutxk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cbwqzanf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hheledmd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mvqyngdo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xcifuezw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rkuaybfn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2estsiovs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2awovzzzo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yacigqhi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hdmcjzls.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mwmsezup.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdehjxap.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cvtsiatx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tsxfqvqn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uephdazc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gxyhevab.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yufwsavj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dgbirbxk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bawztpmn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xabsapdu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jsdzdjtr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mewlzscu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ogrpvyhe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bgnlmtmb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2btkrffhd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bcwmplxv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wnuvckqw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vqlgptpe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rpimlufl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rasvggrf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnbsgcul.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2eccleyez.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hlupyuop.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wkjulros.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2takjufil.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2inbxephy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vtcnikkk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2boxfoqwq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kkjemwdy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xzwadosv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bhildqfs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zugtceya.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bypghvpv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uerwlscl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2sifsxjcd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ingxgtqy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdokxlle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gnndbeim.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bbsecsyy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gblpsuso.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2elihjyzd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2thoxoqaw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gmxdadbf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kmjlipwh.html


<!-- 参考信息 -->