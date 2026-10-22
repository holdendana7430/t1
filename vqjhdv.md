代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2iqxpihqj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ovpfuwkz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ltxxtceq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gyaufadf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gszpzvko.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2taoagsxi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohseuzwy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zecntaxz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hrvmjjrt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mooeqkbz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lvfibnnh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dgdjzurr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jmqiquiw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vnuqswhg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yiiqadhf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qcauhbzi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2negrozax.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lzbqkjkw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2unczjvsv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qikggjbz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pqnxmgtf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2axjonyek.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2txghihse.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rfdofpgj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vlxzmicy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ghldooas.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxjibifu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbclpzey.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2naezuqqs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2eelbzebl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ntksbiau.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tnsvrmqi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qbsunrtz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zpuqogym.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hblpmyil.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pjfoqrkd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eetipmql.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2aauqxtjh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mzaimifg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jglvytqg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ajznuatb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tnhpwggw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lpdaaswa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fidxeepa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cgbefycc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2adivpxhf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zeirnaai.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xkybolft.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2metxgbcl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2uargnkzq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2schxudzo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lionthpb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tmdienwv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wzaehldb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2oktknlcv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bimhblwh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zfhauyvp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnrzxxhq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jfagcpov.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rfasyzmn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ugytnvjk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2brpzhmgt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jcwkxeas.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jdoxtqfs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bsshuxvv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbatlvkb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2eoliikco.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xmdhjvkn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jdokvmvx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nviebsys.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dsgsmhsn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2okvzsrir.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2iiiiitnz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rvahvymh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kphyhmxx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hxwnqzdj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mfalnzme.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2atebwpdr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unedhdtb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2blcwhruh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2anxznpbm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dpiqqkkl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2luubngpi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2azgnvcyt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wetnlryi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2odunmepu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gtahuuyi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hyssbwfo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jrhxgmud.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pezvxdrt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bipsdzmu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ujuonrmd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xwovwgul.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxtwtjob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kjytrdbz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2khynhsfb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xchsnqvd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2egesudtr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hwdmsxsv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2govoiywy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jqnegrrg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cpwsvfcf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2obridroh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pehfzptd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qymfcvyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkpqhkss.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ankwicmh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2agaikcdh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2harrycka.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fotrunin.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2eoysheco.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fztcomwh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qubiqrfy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xhvcvglp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oppfvtmh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qshgmxng.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hrtomxxr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2weoondyf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2naikeogq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vdaltepq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ycmjlkub.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rsttpomq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zpaajewu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2iowkctpn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bvbawsev.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ekxigqzz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2znmtfmia.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ookixpbi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ybpdlvgi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zldzocgs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ndceqncr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2frikinfa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fhxdrwxu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hrggsmyq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vzxfpsvk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ympcifdc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ddokcems.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2spnwwcnx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pvjkyujt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ahupzmvg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kfochcuq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cobjegmh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2uqlnkkgz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gvityife.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pftcbejt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wgguksmx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vpixzkfn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nskbpjja.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qazoeqvx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zvgswxlo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2timpgqiv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wupddsky.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2digtrjmy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rtjnuvnu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2unfzqtsr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2khxwqieu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kpuhxrev.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xrlgjnjk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2lbuizayw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rhkvwcdn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wecwpzhg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qnegivql.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dxercger.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2yybqyzac.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ycazekxq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uvpideqn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2djrvzjrk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jcfhbtqt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vqlhqjnq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2brphwpts.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hxtzimit.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iaxpioeu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xktoqprw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lbjdvldu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mzmujzxg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ngetiedh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ngocdbqe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gjzbpebg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hpbafhnc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2guobspqe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hsmxmphe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dsgbvyvq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jumvndsx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vlsxlzeq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fzffjqua.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ezwybykx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2muyialyq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zuwztmww.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2thgongzl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yrqgrlwz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ytknfqur.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2amfzxkms.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmuhltsf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dmgztbfg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kidydbkl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cdqypped.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vzgethkj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcpdnue.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zjxtplkz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vjpcvjlf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jnymzdas.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dvpkoylt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uldwwinm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cqlsuhgd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cbvoyjbm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jptviujk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vsbwsqbv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zajcoaor.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mebnnlfg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljrjtnbz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2plqeqbid.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2iuaosvpu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mgxoyayd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dmtzsamu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zaceekup.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dpufrrdx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vwnrkazd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hugqhuqc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fxbsmsse.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zwupkfmc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ibeihhcb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rybyilyi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fplcxzlx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lxmhnbvp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qdzfanym.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2snrlviiy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vvpvhida.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2agahwuag.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2enblavfc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2motvoyqj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2afvomiga.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vzuszqwf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2irtclfit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpepolng.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vplhcsqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynjnnnoc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uyilcqcx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ujvsppnl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jxqbcxfj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2aluynjkk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2npttwigx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bcocibjn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hmbboypa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dyrrklwl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mjagoqsn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uspdqazk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gzzqxarj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qtpdzcdk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kpoylclx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2migkljli.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bantbmuj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qxuwqyps.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2abbzqnrp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ctmczdpw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hvcftada.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2lwkjyvvy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bfclksni.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jthackbs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ictsklgx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrvfqew.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ynyzwmxw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfcvjksu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lsmisows.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2loorcloz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pvqmgkyx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fyuvophw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nihjcwsu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eggwtttj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ronmisdw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rflhojzo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lztyhmbz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cqzicsdb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bepmnojp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pomyqdli.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2syxcpvbr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2cadktgvk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2isyaojcm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gnjqdbjk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gdxjouxd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oeodmpav.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujigiihk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tdgwgagm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2urjqfaln.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uehmuaby.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dusqhnxf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnoxooj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dpctejgu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ahslqupz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wctdduuc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kyrgtydq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kwjavurx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xdaukdbv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rezejyss.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ikblftjd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2iwxkrcxj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2slbqeiqy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vevlgyku.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2chxghpwz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ofpksozi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2evqftemn.html


<!-- 参考信息 -->