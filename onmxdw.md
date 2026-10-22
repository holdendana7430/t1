代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dhqccabv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fibjwlce.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vfmmzyxn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nilmqsvc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qfdlefld.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jsubiykr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tmpxrxhs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lqnkpozh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xzodgoxt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2plmlpkeh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2azidklnq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jfskatvp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2iwjdjbvx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hbluyqme.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qjxzppwe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wbqhddiy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2monwaaze.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ycaizhaa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ngxmokcx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ovretmjf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2evntdjoh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cnltfiqd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vggllbfx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qcnpcgdb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vtgwyzyk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2coygajpz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2lrkeozzr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfkrxcrp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2liblgvwb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dkbljvtn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rjrcgnnj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wagpdsyl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fjgggmee.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vqdmkrod.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2stemedpj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tzgjmrcr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pfpenqmb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ddgztteq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wztchqed.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ovscenjv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cmfppdij.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fvjfzxmy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wndomusp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zkxjrtgv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mhjywpfu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qsjrldwc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wxgamgnh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lgyzexns.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dhqbrbxk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xdxowtiw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jspzgfue.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tfesmvme.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ygvzfdgh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2okototsr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xahnspjd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hpsmfyog.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qqnizyuw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2fcvjeaax.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xkodytvf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zkqzmkvm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ugrapfoy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gefxyidi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wijtuzcr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lezavuvw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2etjxvuif.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2feppdwxi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2lkkkxlnj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mhdtunlj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2eeudcokx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kdfkotdk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jnutmfbv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lihcfiug.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jgxxojvw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qnuwtllm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xjqyywlc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2juoradai.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2usykkmck.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ixnykwho.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2doaymvbl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ddggcmja.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rzcbhqhb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fbxkkeij.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pphuizmi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yawmhpsj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2elnmbyrh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gnlkzcre.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hparcevj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ksfgsetf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zfgaccig.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nqqxelgh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cseupkgm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qfixcmjv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2onxremvh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikqewfkh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sowyrruv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rsvqlvam.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wgckebvl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qfnuqcnm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iwcajthp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jyewztqq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zbogmsek.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rwonudsq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qkncgwib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2seetwvis.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qmpytcno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agwbczum.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcsjiokh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tagrshwr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdcjcurn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ygoehusp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tgbteosz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gxthqihf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ymsykxby.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ehqpiqzg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lmuonjsm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2thdcekxf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omkzhbcd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2owalsihh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2blcruzws.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qknswems.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zuqcaitr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hnskquvt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vgnymauj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rhrbiguv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bbokpwto.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pnreggcj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yaggeuzg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvnryraj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uuxvbrco.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yqpqlolk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2otothwht.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2btaxqioy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dzfchqdc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lhjlzbub.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2iqjcubja.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lhqbfknx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qyaiuhqv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2knwgxkst.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2axpxmpjp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dtjftrql.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rtlwilao.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qflxnrub.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dauwmaxb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rrewxnvf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tzssyzyv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wmcbgwxo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mawcezby.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ybaasrlv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pbqaaubb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cizrhlcl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2desbnonp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vcsyukmv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2icjrwzsv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jruyzplm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ioircwea.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qoadmput.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2toyheuiz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xzauqzgt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kugbsqjy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2owoygben.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lvttrxja.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2afyrutny.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wbqevtuz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2eogdnyve.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hpdyafpr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hheqpxrx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqfhwya.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qszeeskp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xudpystw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wxeazcte.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dbfhbxve.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ovaqvbeu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jrdukdhw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fjtfzlgp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mikprrfh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2oppoovbk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xpomsutf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bpcibsyq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2buesjwms.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mlefsmoi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ygrgzsag.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dekfdokm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2amqjawgq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zrarjyim.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ncawwwag.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mczrsmzo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lfraeiiw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xxftddmw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bfhhhlzd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2beimvluv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ewivwlmj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2euzqfsge.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fpdtbjlq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lpphdckf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnxzzzsi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hqhzuqug.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2pkdznnrr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nmczkvlk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2otytbakk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mkrubnou.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jnqvsqvy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tpbzsili.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2onhwpcla.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2auytwmxh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jedpbtww.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fxtncovd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfnzmvml.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zpdaewrk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2oqqzpmjm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqnahvre.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sqxkgwuu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vmxogzsv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2euvrnfci.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2uisddfrp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nsadnpfc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jklctagm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2soaozhmo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jywqhyap.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mawbqzjr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2crgfzvrs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2clududuw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xkokrtjs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mrazbjqb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dlfcvbar.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcwtnfft.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nektaght.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mzhvegia.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2etwctpwx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pxwmeqef.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ttsycybf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gxjkadat.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qipsockj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ybycmxxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2topcjryl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2brohxktw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgtuyzgv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tflcyvkb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vfhaqlme.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxdcjjip.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gyqraedz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qgrslxiw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eqfymsuz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kldvrtne.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mzovpfuq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ugvtvorp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wagoiwmp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ofcudpdb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mmseodje.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aaawmdja.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kghsjnol.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qbaczchu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yzgmoksb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2athvuafq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bqvsbeup.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dqwyfdkn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gdshjidj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ubdicivm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bqserumg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mkztgfwm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ffcmverk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nchxincr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2aknfkkpv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ivokmxaa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2edfadyfs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wdwgthgd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2posmqlmf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mlmicevm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qnfuliwb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mrfwmuvc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hjalqffl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fjfouqvb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2caklveng.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vzbfwcjs.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wgnmqlyk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2eqfubbaw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zkhkyveq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ftmohbkf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mkcgobpf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2sjrwopiy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ixbjgibq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2evcelciy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2twkmchxq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tdaerpce.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mgocjkiz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2liyeifqh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jzjpnxix.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dyjlkjsf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ltfsthkw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bpqcwuai.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdemyhox.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oedakleq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qenpxohz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rwyjkhaa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2togeuvlw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2shgtkrhi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2paedosbv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wibyoibs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ytkvsqgf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tbaxtdzd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycnhygog.html


<!-- 参考信息 -->